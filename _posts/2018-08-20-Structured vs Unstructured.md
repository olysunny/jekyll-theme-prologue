---
title: Structured vs Unstructured
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
<a href="#" class="image fit"><img src="{{ 'assets/images/structured-unstructured.jpg' | relative_url }}" alt="Ipsum Feugiat" /></a>


<h1>How Semi-Structured Data Fits with Structured and Unstructured Data</h1>

Semi-structured data maintains internal tags and markings that identify separate data elements, which enables information grouping and hierarchies. Both documents and databases can be semi-structured. This type of data only represents about 5-10% of the structured/semi-structured/unstructured data pie, but has critical business usage cases.

Semi-structured data maintains internal tags and markings that identify separate data elements, which enables information grouping and hierarchies. Both documents and databases can be semi-structured. This type of data only represents about 5-10% of the structured/semi-structured/unstructured data pie, but has critical business usage cases.

Email is a very common example of a semi-structured data type. Although more advanced analysis tools are necessary for thread tracking, near-dedupe, and concept searching; email’s native metadata enables classification and keyword searching without any additional tools.

<div class="6u$ 12u$(small)">
		<h3>Examples of Semi-structured Data</h3>
		<ul>
			<li><b>Markup language XML</b> This is a semi-structured document language. XML is a set of document encoding rules that defines a human- and machine-readable format. Its value is that its tag-driven structure is highly flexible, and coders can adapt it to universalize data structure, storage, and transport on the Web.</li>
			<li><b>Open standard JSON (JavaScript Object Notation)</b> JSON is another semi-structured data interchange format. Java is implicit in the name but other C-like programming languages recognize it. Its structure consists of name/value pairs (or object, hash table, etc.) and an ordered value list (or array, sequence, list). Since the structure is interchangeable among languages, JSON excels at transmitting data between web applications and servers.</li>
	               <li><b>NoSQL</b> Semi-structured data is also an important element of many NoSQL (“not only SQL”) databases. NoSQL databases differ from relational databases because they do not separate the organization (schema) from the data. This makes NoSQL a better choice to store information that does not easily fit into the record and table format, such as text with varying lengths. It also allows for easier data exchange between databases. Some newer NoSQL databases like MongoDB and Couchbase also incorporate semi-structured documents by natively storing them in the JSON format.</li>
          </ul>
	</div>
</div>

In big data environments, NoSQL does not require admins to separate operational and analytics databases into separate deployments. NoSQL is the operational database and hosts native analytics tools for business intelligence. In Hadoop environments, NoSQL databases ingest and manage incoming data and serve up analytic results.

These databases are common in big data infrastructure and real-time Web applications like LinkedIn. On LinkedIn, hundreds of millions of business users freely share job titles, locations, skills, and more; and LinkedIn captures the massive data in a semi-structured format. When job seeking users create a search, LinkedIn matches the query to its massive semi-structured data stores, cross-references data to hiring trends, and shares the resulting recommendations with job seekers. The same process operates with sales and marketing queries in premium LinkedIn services like Salesforce. Amazon also bases its reader recommendations on semi-structured databases.
