⚡ Electricity Meter Reading Management System
📌 Overview

The Electricity Meter Reading Management System is a desktop-based application designed to record, manage, and view daily electricity meter readings efficiently.
It helps users track electricity consumption per meter, avoid duplicate entries, and maintain accurate historical records.

This system is built following a layered architecture (DAL / BLL / UI) and uses Oracle Database for reliable data storage.

🚀 Features

🔢 Add daily electricity meter readings

📅 Select readings by date

🔍 View readings in a grid (daily view)

🧾 Prevent duplicate meter readings

🕒 Automatic date & time handling

🖱️ Load meter details using grid double-click

📊 Display historical meter readings

🔐 User-based meter access

🛠️ Technologies Used

C# (.NET Framework)

WinForms

Oracle Database

DevExpress GridControl

ADO.NET

Layered Architecture (DAL / BLL / UI)

🧱 Project Architecture

The application follows a 3-layer architecture:

UI Layer        → Forms, GridControls, User Interaction
Business Layer  → Validation, Business Rules
Data Layer      → Oracle DB Access (Queries, Readers)


This separation makes the system:

Easy to maintain

Easy to debug

Scalable for future features

🗄️ Database Design

Main tables used:

cdl_electricity_readings

cdl_elecreading_view

cdl_electricity_meters

cdl_elemeter_users

Key fields:

Meter Number

Reading Date

Reading Time

Current Reading

Maximum Demand

User Access Status

🖥️ Screens & Functionality

Date selection loads available meter readings

Grid row click fills form fields automatically

Double-click meter selection loads meter number & location

Time defaults to current time when no record exists

⚠️ Validations

Prevents empty meter number submission

Prevents duplicate readings for the same date

Ensures correct date sequence

Handles null database values safely

📦 How to Run the Project

Clone the repository

Open solution in Visual Studio

Configure Oracle DB connection

Restore required NuGet packages

Run the project


👤 Author

Sachindra Samadhi
BSc (Hons) in Information Technology
Software Engineer

📄 License

This project is for learning and internal use.
