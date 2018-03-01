# selenium-Python
# coding:utf-8
from selenium import webdriver

option = webdriver.ChromeOptions()
option.add_argument('headless')  # 静默模式
# 打开chrome浏览器
driver = webdriver.Chrome( chrome_options=option)
driver.get("https://guides.github.com")
print(driver.title)
