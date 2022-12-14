# Xpath
Selecting Web Elements from the DOM is an essential skill for automating web pages. There are a lot of ways to do Xpath and there is no always best solution. Try to answer the following questions by using Xpath. In chrome console, you can do $x("some xpath")to select these elements. This cheatsheet is also very helpful https://devhints.io/xpath . $x returns an array of elements. Save all your Xpath queries in text file. You should try to do it individually but seek hints from others if you get stuck. Compare queries with your teammates as there are many ways to write these.


## Employee Overview
- Select all tds that have money sign in them
  - Solution: 
  - $x("//td[contains(text(),'$')]")
- Get the first tr in the tbody
  - Solution: 
  - $x("//tbody//tr[1]")
- Get the last tr in the tbody
  - Solution: 
  - $x("//tbody//tr[last()]")
- Get All tds where the id is between 200 and 300
  - Solution:
  - $x("//td[@id < 300 and @id > 200]")


## Hi Score
- Get the li that contains TIM's Dig Dug score
  - Solution:
  - $x("//li[contains(text(),'Dig Dug') and contains(text(), 'TIM')]")
- Get the list items that belong to YVN or GAR
  - Solution:
  - $x("//li[contains(text(),'YVN') or contains(text(), 'GAR')]")
- Get the total amount of li in the document
  - Solution:
  - $x("count(//li)")

## Sales Report
- Select only the second table
  - Solution:
  - $x("//div[position()=2]/table[position()=1]")
- Select all trs where the attribute data-leader="Margaret"
  - Solution:
  - $x("//tr[@data-leader='Margaret']")
- Select all the tds containing the sales where Westview Middle was the troop
  - Solution:
  - $x("//td[contains(text(),'Westview Middle')]")
- Select the last tr of Thin Mints in the first half
  - Solution:
  - 