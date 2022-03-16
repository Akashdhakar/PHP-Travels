from locators.locator import loc

class price():
    def __init__(self,driver):
        self.driver = driver
        self.eml = loc.eml
        self.pss = loc.pss
        self.clk = loc.clk



    def price1(self,eml,ps):
        self.driver.find_element_by_xpath(self.eml).send_keys(eml)
        self.driver.find_element_by_xpath(self.pss).send_keys(ps)
        self.driver.find_element_by_xpath(self.clk).click()