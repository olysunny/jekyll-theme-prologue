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

<h2>unstructured data</h2>
	<div class="row">
		<div class="6u 12u$(small)">
			
			<h3>Typical human-generated</h3>
			<ul>
				<li>Text files: Word processing, spreadsheets, presentations, email, logs.</li>
        <li>Email: Email has some internal structure. However, its message field is unstructured and traditional analytics tools cannot parse it.</li>
        <li>Social Media: Data from Facebook, Twitter, LinkedIn.</li>
        <li>Website: YouTube, Instagram, photo sharing sites.</li>
        <li>Mobile data: Text messages, locations.</li>
        <li>Communications: Chat, IM, phone recordings, collaboration software.</li>
        <li>Media: MP3, digital photos, audio and video files.</li>
        <li>Business applications: MS Office documents, productivity applications.</li>
			</ul>
		</div>
		<div class="6u$ 12u$(small)">
			<h3>Typical machine-generated</h3>
			<ul>
        <li>Satellite imagery: Weather data, land forms, military movements.</li>
        <li>Scientific data: Oil and gas exploration, space exploration, seismic imagery, atmospheric data.</li>
        <li>Digital surveillance: Surveillance photos and video.</li>
        <li>Sensor data: Traffic, weather, oceanographic sensors.</li>
			</ul>
		</div>
	</div>



