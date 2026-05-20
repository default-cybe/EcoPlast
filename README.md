<div align="center">
      <h1><img src="https://raw.githubusercontent.com/default-cybe/EcoPlast/main/ep/static/images/logo.png" width="80px"><br/>EcoPlast</h1>
     </div>
<p align="center"> <a href="https://github.com/default-cybe" target="_blank"><img alt="" src="https://img.shields.io/badge/Website-EA4C89?style=normal&logo=dribbble&logoColor=white" style="vertical-align:center" /></a> <a href="https://twitter.com/default_yt_" target="_blank"><img alt="" src="https://img.shields.io/badge/Twitter-1DA1F2?style=normal&logo=twitter&logoColor=white" style="vertical-align:center" /></a> <a href="https://www.instagram.com/kaivalya_ahir" target="_blank"><img alt="" src="https://img.shields.io/badge/Instagram-E4405F?style=normal&logo=instagram&logoColor=white" style="vertical-align:center" /></a> <a href="https://www.linkedin.com/in/kaivalya-ahir/" target="_blank"><img alt="" src="https://img.shields.io/badge/LinkedIn-0077B5?style=normal&logo=linkedin&logoColor=white" style="vertical-align:center" /></a> </p>

# Description
EcoPlast connects four kinds of people around plastic waste: customers who want to get rid of it, collectors who pick it up and resell it, recycling companies that need a steady supply of raw material, and sellers who make products out of recycled plastic. The point is to keep that plastic moving through the loop instead of into a landfill, and to let everyone in the chain make something out of the deal.

# What it does

- Customers hand off their plastic waste instead of binning it.
- Collectors get paid for picking it up and passing it along.
- Recycling companies buy that plastic as raw material.
- Sellers list products made from recycled plastic.

It's all one Django app, so accounts, orders and the whole buy/sell flow live on the server side. Payments go through Paytm.


# Tech Used
 ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Django](https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white) ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E) ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![Bootstrap](https://img.shields.io/badge/bootstrap-%23563D7C.svg?style=for-the-badge&logo=bootstrap&logoColor=white)
      
# Installation

EcoPlast is a Django project backed by a MySQL database. You will need Python 3 and MySQL installed before you start.

**1. Clone the repository**

	git clone https://github.com/default-cybe/EcoPlast.git
	cd EcoPlast

**2. Create and activate a virtual environment**

	python -m venv venv
	# Windows
	venv\Scripts\activate
	# macOS / Linux
	source venv/bin/activate

**3. Install the dependencies**

	pip install -r requirements.txt

**4. Set up the database**

Create a MySQL database named `EcoPlast` and import the provided schema:

	mysql -u root -p EcoPlast < Database/EcoPlast.sql

**5. Configure environment variables**

Copy the example file and fill in your own values. The application reads all secrets (Django secret key, database credentials, Paytm gateway keys and email settings) from these variables.

	cp .env.example .env

Load the variables into your shell before running the server, or use a tool such as `python-dotenv`.

**6. Run the development server**

	python manage.py runserver

The application will be available at http://127.0.0.1:8000/.

# License

This project is released under the [MIT License](LICENSE).

