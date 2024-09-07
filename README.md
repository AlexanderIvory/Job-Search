# Job-Search
To search jobs on job board websites given a field, outputting the salary ranges and qualifications/experience required.

## To-do:
- Install Scrapy:
	- Run pip install scrapy to install the Scrapy framework.
- Create a Scrapy Project:
	- In your terminal, navigate to your desired directory and run scrapy startproject seek_jobs.
- Generate a Spider:
	- Inside your project directory, create a spider using scrapy genspider job_spider seek.com.
- Configure Spider:
	- Edit the generated job_spider.py file:
		- Set the start_urls to Seek’s job search page.
		- Define the parse method to handle the HTML response and extract job details.
- Define Item Structure:
	- Create an items.py file to define the data fields you want to scrape (e.g., job title, company, location).
- Parse Job Listings:
	- In the parse method, use Scrapy’s selectors (XPath or CSS) to extract job details.
	- Implement logic to filter jobs based on your conditions.
- Handle Pagination:
	- Add logic in the parse method to follow pagination links and scrape multiple pages.
- Store Data:
	- Use Scrapy’s pipelines to save the filtered job data to a file (e.g., CSV, JSON) or a database.
