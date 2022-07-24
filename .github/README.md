# Q-CTRL Front-end Challenge

The Q-CTRL Front-end Challenge is a way for applicants to roles within the Q-CTRL Front-end Engineering team to demonstrate their skills and overall approach to front-end application development.

The requirements are intentionally sparse (the devil is in the detail). We don't want you to do a lot, but what you do should be your best work and should clearly demonstrate you embody [the three virtues](https://thethreevirtues.com/).

## The rules

- Read and understand [the challenge](#the-challenge).
- Create a solution that satisfies [the requirements](#the-requirements).
- Use [REST Countries](https://restcountries.com/) to get all the data you need.
- Write your own pagination logic.
- Write your own search logic (you're not marked on how advanced your search algorithm is).
- Feel free to use a UI library such as [MUI](https://mui.com/).
- Spend no more than three hours on this challenge.
- Send us a link to the repository containing your solution when you're done.

## The challenge

Build a [React](https://reactjs.org/) app that displays a list of [countries](https://github.com/qctrl/front-end-challenge/blob/master/assets/countries.png) with the capability of filtering results through a search mechanism, paginating countries, and showing information about each individual [country](https://github.com/qctrl/front-end-challenge/blob/master/assets/country.png).

## The requirements

```
Feature: View the countries page

  Scenario: Countries are loading
    Given I am on the countries page
    Then I should see a loading spinner

  Scenario: Countries have loaded
    Given I am on the countries page
    When the countries have finished loading
    Then I should see the first 10 countries in alphabetical order
    And I should not see the previous button

Feature: Browse countries on the countries page

  Scenario: Click the next button
    Given I am on the countries page
    And I am not on the last page of countries
    When I click the next button
    Then I should see the next 10 countries

  Scenario: Click the previous button
    Given I am on the countries page
    And I am not on the first page of countries
    When I click the previous button
    Then I should see the previous 10 countries

  Scenario: Viewing the first page
    Given I am on the countries page
    When I am on the first page of countries
    Then I should not see the previous button

  Scenario: Viewing the last page
    Given I am on the countries page
    When I am on the last page of countries
    Then I should not see the next button

Feature: Search countries on the countries page

  Scenario: Search countries
    Given I am on the countries page
    And I have entered some text in the search box
    When I click the search button
    Then I should see a list of countries that match my search

Feature: View the country page

  Scenario: Clicking a country
    Given I am on the countries page
    When I click a country
    Then I should see the country page

  Scenario: Country is loading
    Given I am on the country page
    Then I should see a loading spinner

  Scenario: Country has loaded
    Given I am on the country page
    When the country has finished loading
    Then I should see a back button
    And I should see the country's flag
    And I should see the country's name
    And I should see the country's population
    And I should see the country's demonym

  Scenario: Click the back button
    Given I am on the country page
    When I click the back button
    Then I should see the countries page 
```

## Contributing

See [Contributing](https://github.com/qctrl/.github/blob/master/CONTRIBUTING.md).

## Credits

See [Contributors](https://github.com/qctrl/front-end-challenge/graphs/contributors).

## License

See [LICENSE](https://github.com/qctrl/front-end-challenge/blob/master/LICENSE).
