<p style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong><u><span style="font-size:24px;line-height:107%;">Cafe API</span></u></strong></p>
<p style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'>This repository contains the source code for a RESTful API that manages information about cafes. Developers can use this API to perform various operations such as retrieving a list of all cafes, getting a random cafe, searching for cafes based on location, adding a new cafe, updating the coffee price of a cafe, and deleting a cafe by its ID. The API follows RESTful routing principles for a well-organized and predictable structure.</p>
<p style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>Technologies Used</strong></p>
<ul style="margin-bottom:0cm;margin-top:0cm;" type="disc">
    <li style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>Flask:</strong> A lightweight web framework for building the API.</li>
    <li style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>SQL Alchemy:</strong> A SQL toolkit and Object-Relational Mapping (ORM) library for working with databases.</li>
    <li style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>Postman:</strong> A popular API testing tool for testing and exploring the functionality of the API.</li>
</ul>
<p style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>Getting Started</strong></p>
<ol style="margin-bottom:0cm;margin-top:0cm;" start="1" type="1">
    <li style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'>Clone the repository:</li>
</ol>
<p style='margin-top:0cm;margin-right:0cm;margin-bottom:10.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;git clone <a href="https://github.com/Siya016/Cafe-Api.git">https://github.com/Siya016/Cafe-Api.git</a></p>
<div style='margin-top:0cm;margin-right:0cm;margin-bottom:10.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'>
    <ol style="margin-bottom:0cm;list-style-type: undefined;">
        <li style='margin-top:0cm;margin-right:0cm;margin-bottom:10.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'>Install dependencies:</li>
    </ol>
</div>
<p style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;pip install -r requirements.txt</p>
<ol style="margin-bottom:0cm;margin-top:0cm;" start="3" type="1">
    <li style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'>Set up the database:</li>
</ol>
<p style='margin-top:0cm;margin-right:0cm;margin-bottom:10.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; flask db init</p>
<p style='margin-top:0cm;margin-right:0cm;margin-bottom:10.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; flask db migrate</p>
<p style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; flask db upgrade</p>
<ol style="margin-bottom:0cm;margin-top:0cm;" start="4" type="1">
    <li style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'>Run the application:</li>
</ol>
<p style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;flask run</p>
<p style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>API Endpoints</strong></p>
<p style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>1. Get All Cafes</strong></p>
<ul style="margin-bottom:0cm;margin-top:0cm;" type="disc">
    <li style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>Endpoint:</strong> <strong>GET /cafes</strong></li>
    <li style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>Description:</strong> Retrieve a list of all cafes.</li>
</ul>
<p style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>2. Get Random Cafe</strong></p>
<ul style="margin-bottom:0cm;margin-top:0cm;" type="disc">
    <li style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>Endpoint:</strong> <strong>GET /cafes/random</strong></li>
    <li style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>Description:</strong> Get information about a randomly selected cafe.</li>
</ul>
<p style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>3. Search Cafe by Location</strong></p>
<ul style="margin-bottom:0cm;margin-top:0cm;" type="disc">
    <li style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>Endpoint:</strong> <strong>GET /cafes/search?location={location}</strong></li>
    <li style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>Description:</strong> Search for cafes based on their location. The <strong>location</strong> parameter allows filtering by a specific geographical area.</li>
</ul>
<p style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>4. Post New Cafe</strong></p>
<ul style="margin-bottom:0cm;margin-top:0cm;" type="disc">
    <li style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>Endpoint:</strong> <strong>POST /cafes</strong></li>
    <li style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>Description:</strong> Add a new cafe to the system. Requires providing details such as name, location, and coffee price.</li>
</ul>
<p style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>5. Update Coffee Price</strong></p>
<ul style="margin-bottom:0cm;margin-top:0cm;" type="disc">
    <li style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>Endpoint:</strong> <strong>PUT /cafes/{id}/price</strong></li>
    <li style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>Description:</strong> Update the price of coffee for a specific cafe identified by its unique ID. Requires providing the new coffee price.</li>
</ul>
<p style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>6. Delete Cafe by ID</strong></p>
<ul style="margin-bottom:0cm;margin-top:0cm;" type="disc">
    <li style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>Endpoint:</strong> <strong>DELETE /cafes/{id}</strong></li>
    <li style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'><strong>Description:</strong> Delete a cafe from the system based on its unique ID.</li>
</ul>
<p style='margin-top:0cm;margin-right:0cm;margin-bottom:10.0pt;margin-left:0cm;line-height:120%;font-size:14px;font-family:"Calibri",sans-serif;'>&nbsp;</p>
<p style='margin-top:0cm;margin-right:0cm;margin-bottom:8.0pt;margin-left:0cm;font-size:11.0pt;font-family:"Calibri",sans-serif;'><strong><span style='font-size:16px;font-family:"Calibri",sans-serif;'>&nbsp;</span></strong></p>
