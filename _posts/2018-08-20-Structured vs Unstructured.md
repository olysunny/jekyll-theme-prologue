---
title: Structured vs Unstructured Data
author: Max
layout: post
---

Structured data is comprised of clearly defined data types whose pattern makes them easily searchable; while unstructured data is usually not as easily searchable, including formats like audio, video, and social media postings.

<h1>What is Structured Data?</h1>
Structured data usually resides in relational databases (RDBMS). Fields store length-delineated data phone numbers, Social Security numbers, or ZIP codes. Even text strings of variable length like names are contained in records, making it a simple matter to search. Data may be human- or machine-generated as long as the data is created within an RDBMS structure. This format is eminently searchable both with human generated queries and via algorithms using type of data and field names, such as alphabetical or numeric, currency or date.

Common relational database applications with structured data include airline reservation systems, inventory control, sales transactions, and ATM activity. Structured Query Language (SQL) enables queries on this type of structured data within relational databases.

Some relational databases do store or point to unstructured data such as customer relationship management (CRM) applications. The integration can be awkward at best since memo fields do not loan themselves to traditional database queries. Still, most of the CRM data is structured.


<h1>What is Unstructured Data?</h1>
Unstructured data is essentially everything else. Unstructured data has internal structure but is not structured via pre-defined data models or schema. It may be textual or non-textual, and human- or machine-generated. It may also be stored within a non-relational database like NoSQL.

Typical human-generated unstructured data includes:

Text files: Word processing, spreadsheets, presentations, email, logs.
Email: Email has some internal structure thanks to its metadata, and we sometimes refer to it as semi-structured. However, its message field is unstructured and traditional analytics tools cannot parse it.
Social Media: Data from Facebook, Twitter, LinkedIn.
Website: YouTube, Instagram, photo sharing sites.
Mobile data: Text messages, locations.
Communications: Chat, IM, phone recordings, collaboration software.
Media: MP3, digital photos, audio and video files.
Business applications: MS Office documents, productivity applications.
Typical machine-generated unstructured data includes:

Satellite imagery: Weather data, land forms, military movements.
Scientific data: Oil and gas exploration, space exploration, seismic imagery, atmospheric data.
Digital surveillance: Surveillance photos and video.
Sensor data: Traffic, weather, oceanographic sensors.
