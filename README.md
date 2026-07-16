# FridgeFrenzy — Fridge Management System

An all-in-one fridge management application that streamlines fridge maintenance, fault reporting, and inventory/procurement for a beverage manufacturer, paired with an e-commerce platform. Built with **ASP.NET Core MVC**.

Developed as part of **ONT3010: Project III** at Nelson Mandela University.

## Background

Beverage manufacturers supply fridges to customers (e.g. spaza shops, shebeens) to ensure proper refrigeration of their products. This system replaces manual, paper-based processes for customer management, inventory control, fault reporting, servicing, and supplier procurement with a streamlined web-based solution.

## Subsystems

| Subsystem | Description |
|---|---|
| **Administration** | Core subsystem managing customers, employees, locations, fridges, and suppliers |
| **Customer Management** | Manages customer data, fridge allocations, stock levels, and internal purchase requests |
| **Fridge Fault** | Handles fault reporting from customers and repair scheduling by fault technicians |
| **Fridge Maintenance** | Manages scheduled maintenance visits and service history, visible to both technicians and customers |
| **Purchasing** | Manages suppliers, quotations, purchase orders, and delivery notes |

## Actors / Users
- Administrator
- Customer Liaison
- Inventory Liaison
- Customer
- Fault Technician
- Maintenance Technician
- Purchasing Manager
- Supplier

## Key Features
- **PayPal payment integration** for the e-commerce checkout flow
- **Role-based authentication** to enforce access control across the different actors/user types
- **GUIDs** used for unique entity identification across the system

## Tech Stack
- **Backend:** ASP.NET Core MVC (C#)
- **Frontend:** HTML, CSS, JavaScript
- **Database:** SQL Server
- **Payments:** PayPal (sandbox integration)

## Setup
1. Clone the repo
2. Add your own connection string and PayPal credentials via `appsettings.Development.json` (not committed) or User Secrets — see `appsettings.json` for the expected structure
3. Run database migrations
4. `dotnet run`

## Credits
Project coordinator: Mr Bongani Mngaza, Nelson Mandela University
