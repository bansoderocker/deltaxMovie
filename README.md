# deltaxMovie

-- creating database
Create Database deltax

-- creating table to store data
USE [deltax]
GO

/****** Object:  Table [dbo].[movie]    Script Date: 05/07/2022 19:19:38 ******/
SET ANSI_NULLS ON
GO

SET QUOTED_IDENTIFIER ON
GO

Create Database deltax

use deltax
GO

CREATE TABLE [dbo].[movie](
	[ID] [int] IDENTITY(1,1) NOT NULL,
	[Mname] [varchar](100) NULL,
	[Rdate] [datetime] NULL,
	[Producer] [varchar](50) NULL,
	[Actor] [varchar](500) NULL,
	[Lastupdated] [datetime] NULL
) ON [PRIMARY]

GO

--- insert query 
insert into deltax.dbo.movie (Mname,Rdate,Producer,Actor,Lastupdated)
values(@Mname,@Rdate,@Producer,@Actor,GETDATE())


select * from deltax.dbo.movie

--delete deltax.dbo.movie where ID = 2

----- store porcedure used in API

USE [deltax]
GO

/****** Object:  Table [dbo].[movie]    Script Date: 05/07/2022 19:19:38 ******/
SET ANSI_NULLS ON
GO

SET QUOTED_IDENTIFIER ON
GO

SET ANSI_PADDING ON
GO

CREATE TABLE [dbo].[movie](
	[ID] [int] IDENTITY(1,1) NOT NULL,
	[Mname] [varchar](100) NULL,
	[Rdate] [datetime] NULL,
	[Producer] [varchar](50) NULL,
	[Actor] [varchar](500) NULL,
	[Lastupdated] [datetime] NULL
) ON [PRIMARY]

GO

SET ANSI_PADDING OFF
GO

