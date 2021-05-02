#BestBuyBot
from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.support.ui import WebDriverWait
from selenium.webdriver.support import expected_conditions as EC
import time
driver = webdriver.Chrome()
#Type in url here
driver.get("any url from bestbuy")
usernameStr = ''
passwordStr = ''
firstName = ""
lastName = ""
address = ""
city = ""
zipCode = ""
creditCard = ""
dropDownState = ""
cardNum = ""

print (driver.title)
print (driver.current_url)
buyButton = False
while not buyButton:
	try:
		addToCartBtn = addButton = 
driver.find_element_by_class_name("btn-disabled")
		print("Button is not ready")
		time.sleep(1)
		driver.refresh()
	except:
		addToCartBtn = addButton = driver.find_element_by_class_name("btn-primary")
		print("Button was clicked")
		addToCartBtn.click()
		buyButton = True
		driver.get("https://www.bestbuy.com/cart")
		time.sleep(3)
		driver.find_element_by_css_selector(".btn-primary").click()		
		time.sleep(3)
		#driver.get("https://www.bestbuy.com/identity/signin?token=tid%3A6c2647a7-7245-11eb-9b23-005056ae0065")
		username = driver.find_element_by_id("fld-e")
		username.send_keys(usernameStr)
		passwordName = driver.find_element_by_id("fld-p1")
		passwordName.send_keys(passwordStr)
		driver.find_element_by_class_name("btn-secondary").click()
		time.sleep(3)
		driver.get("https://www.bestbuy.com/checkout/r/fulfillment")
		driver.find_element_by_class_name("btn-lg").click()
		time.sleep(3)
		driver.get("https://www.bestbuy.com/checkout/r/payment")
		firstNameEnter = driver.find_element_by_id("payment.billingAddress.firstName")
		firstNameEnter.send_keys(firstName)
		lastNameEnter = driver.find_element_by_id("payment.billingAddress.lastName")
		lastNameEnter.send_keys(lastName)
		addressEnter = driver.find_element_by_id("payment.billingAddress.street")
		addressEnter.send_keys(address)
		cityEnter = driver.find_element_by_id("payment.billingAddress.city")
		cityEnter.send_keys(city)
		zipCodeEnter = driver.find_element_by_id("payment.billingAddress.zipcode")
		zipCodeEnter.send_keys(zipCode)
		dropDown = driver.find_element_by_id("payment.billingAddress.state")
		dropDown.send_keys(dropDownState)
		#cardNumEnter = driver.find_element_by_id("optimized-cc-card-number")
		#dropDown.send_keys(cardNum)
		driver.find_element_by_class_name("btn-lg").click()
		
#driver.quit()
