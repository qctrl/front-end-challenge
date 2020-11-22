# Q-CTRL Front-end Engineering Challenge

The Q-CTRL Front-end Engineering Challenge is a way for applicants to roles within the Q-CTRL Front-end Engineering team to demonstrate their skills and overall approach to front-end application development.

The requirements are intentionally sparse (the devil is in the detail). We don't want you to do a lot, but what you do should be your best work and should clearly demonstrate you embody the [Three Virtues](http://threevirtues.com/).

## Table of Contents

- [Q-CTRL Front-end Engineering Challenge](#q-ctrl-front-end-engineering-challenge)
  - [Table of Contents](#table-of-contents)
  - [The Rules](#the-rules)
  - [The Challenge](#the-challenge)
  - [The Requirements](#the-requirements)
    - [Countries Page](#countries-page)
    - [Country Page](#country-page)
  - [Additional Information](#additional-information)
    - [Assets](#assets)
  - [Contributing](#contributing)
  - [Credits](#credits)
  - [License](#license)

## The Rules

- Read and understand [The Challenge](#the-challenge)
- Create solutions that satisfy [The Requirements](#the-requirements)
- Send a link to the repository containing your solution to careers@q-ctrl.com
- Write your own pagination logic
- Write your own search logic, you are not marked on how advanced your search algorithm is
- Try not to spend more than 3 hours
- You are free to use a UI library such as [Material-UI](https://material-ui.com/)

## The Challenge

We want to build an app that can display a list of countries with the capability of filtering results through a search mechanism, paginating countries and showing information about each individual country.

## The Requirements

### Countries Page

The first feature is to create a page where a customer can view all the countries that are returned from the countries API. Create a web application using [React](https://reactjs.org/) that satisfies the following scenarios:

```text
Scenario 1: Countries loading
When I visit the Countries page
Then I should see a loading spinner

Scenario 2: Countries loaded
Given I am on the countries page
When the countries have finished loading
Then I should see the first 10 countries in alphabetical order
And display their country name

Scenario 3: Click previous page
Given I am on the Countries page
And I am not already on the first page
When I click on the previous button
Then I should see the previous 10 countries in alphabetical order

Scenario 4: Click next page
Given I am on the Countries page
And I am not already on the last page
When I click on the next button
Then I should see the next 10 countries in alphabetical order

Scenario 5: Search
Given I am on the Countries page
When I enter text in the search text input
And when I click search
Then I should check if the country's name contains the search text

Scenario 6: No next page
Given there are no more countries on the next page
When either after a search or navigating to a new page
Then hide the next page button

Scenario 7: No previous page
Given there are no more countries on the prior page
When either after a search or navigating to a new page
Then hide the previous page button

Scenario 8: Clicking a country
Given the countries have loaded
When I click a country
Then take me to the country page
```

### Country Page

```text
Scenario 1: Country loading
When I visit the Country page
Then I should see a loading spinner

Scenario 2: Country loaded
Given I am on the countries page
When the countries have finished loading
Then I should see the country's flag
And the country's population
And the country's demonym
```

## Additional Information

### Assets

The below assets have been provided to help complete the challenge.

| Name                                              | Description                                                                                      |
| ------------------------------------------------- | ------------------------------------------------------------------------------------------------ |
| [Countries View.png](assets/Countries%20View.png) | Mock up for the Countries View                                                                      |
| [Country View.png](assets/Country%20View.png)     | Mock up for the Country View                                                                         |

## Contributing

See [Contributing](https://github.com/qctrl/.github/blob/master/CONTRIBUTING.md).

## Credits

See [Contributors](https://github.com/qctrl/front-end-challenge/graphs/contributors).

## License

See [LICENSE](LICENSE).
