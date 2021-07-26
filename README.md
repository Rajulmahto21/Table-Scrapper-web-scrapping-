# Table-Scrapper-web-scrapping-
This is a python script which will help you to scrap out table from any HTML based websites on the internet.Sometimes while creating a script ,project or system we need some data from a website or a web page which may be in the form of tables,some script require a .CSV or a list of data were required in order for them to work.So,this python script will help users to scrap tables from the web pages and automatically convert them to .CSV files so that it can be used in the projects or databases.This will include the following :

* Entering the URL
* Entering the required information to scrap out tables
* Converting them to DataFrame
* Finally converting them to .CSV file

<b>Advantages of this script</b>

* It will be really efficient to scrap out tables in just seconds.
* It will save a lot of time.
* Users can also get the updated tables which they could not get if they copy or manually enter data.
* Programmers can get to know more about "WEB SCRAPPING" from this script.

# Prequsites
* Python
   * IDE (Jupyter Notebook is the recommended IDE )
* Python Libraries
   * Selenium
   * Pandas
* Web Driver (of your browser you are going to use recommended is google chrome)

# Installation
* Python : [https://www.python.org/downloads](https://www.python.org/downloads)
* IDE : [https://www.anaconda.com/products/individual](https://www.anaconda.com/products/individual) (followed by installation of jupyter notebook)
* Libraries: Open the directory of your installed python version and type the following lines followed by pressing enter
    * For Selenium: `pip install selenium`
    * For Pandas: `pip install pandas`
* Web Driver : [https://www.selenium.dev/downloads](https://www.selenium.dev/downloads)
   * Open the above link and scroll down to "Browser" now click on the documentation link of your browser here i will show for google chrome.![1](https://github.com/Rajulmahto21/Table-Scrapper-web-scrapping-/blob/main/Snips/1.PNG)
   * Now download the  ChromeDriver 91.0.4472.101 (recommended).![2](https://github.com/Rajulmahto21/Table-Scrapper-web-scrapping-/blob/main/Snips/2.PNG)
   * Now extract the zip and remember the path of extracted chrome driver.

# Setting Up
* Download the Table Scrapper.py file from above and open it in jupyter notebook.
* Now write the path where you extracted the google chrome web driver in place of "your_webdriver_path".
    * `driver = webdriver.Chrome("C:\webdrivers\chromedriver.exe")`
* Now write the URL of the website in which the table to be scrapped is present in place of "your_website_url"
   * `driver.get('https://www.nirfindia.org/2020/UniversityRanking.html')`
* Now write the Xpath of the columns in place of "your_xpath_column_1" which you want to have in your csv file table and write all the xpath of column if you dont know to write the xpath you can refer to google or youtube or refer the example i have shown in how to use section.
   * `column_1 = driver.find_elements_by_xpath('//table[@id="tbl_overall"]/tbody/tr/td[1]')`
