# Q-CTRL Front-end Engineering Challenge

The Q-CTRL Front-end Engineering Challenge is a way for applicants to roles within the Q-CTRL Front-end Engineering team to demonstrate their skills and overall approach to front-end application development.

The requirements are intentionally sparse (the devil is in the detail). We don't want you to do a lot, but what you do should be your best work and should clearly demonstrate you embody the [Three Virtues](http://threevirtues.com/).

## Table of Contents

- [The Rules](#the-rules)
- [The Challenge](#the-challenge)
- [The Requirements](#the-requirements)
  - [Controls Page](#controls-page)
  - [Documentation Page](#documentation-page)
- [Additional Information](#additional-information)
- [Contributing](#contributing)
- [Credits](#credits)
- [License](#license)

## The Rules

- Read and understand [The Challenge](#the-challenge)
- Create solutions that satisfy [The Requirements](#the-requirements)
- Send a link to the repository containing your solution to careers@q-ctrl.com

## The Challenge

There's a new set of product features being planned for [BLACK OPAL](https://q-ctrl.com/products/black-opal/) whereby a customer will be able to create and manage quantum controls. You can think of these controls as being the individual inputs a customer may employ to manipulate their quantum system using the [Q-CTRL App](https://app.q-ctrl.com/). Alongside these new features will be a new documentation website.

## The Requirements

### Controls Page

The first feature in the sprint is to create a page where a customer can view all the controls they have created. Create a web application using [React](https://reactjs.org/) that satisfies the following scenarios:

```
Scenario 1: Controls loading
When I visit the Controls page
Then I should see a loading spinner

Scenario 2: Controls loaded
Given I am on the Controls page
When the controls have finished loading
Then I should see all my controls

Scenario 3: Error loading controls
Given I am on the Controls page
And the controls are loading
When the controls cannot be loaded
Then I should see an error
And I should see a button to try again

Scenario 4: Try loading controls again
Given I am on the Controls page
And there has been an error loading controls
When I click the try again button
Then I should see a loading spinner
And the controls should start to load again
```

### Documentation Page

The second feature in the sprint is to create the new documentation home page. Unlike the React app above, the documentation is a publicly available source of information and must be highly accessible. Using the supplied [design](assets/documentation.pdf), create the **HTML only** for the design. No CSS, No JS, no frameworks - just plain old semantic HTML (POSH).

The purpose of this component of the Q-CTRL Front-end Engineering Challenge is to determine your grasp of valid, standards-compliant, semantic HTML - a skill that has become surprisingly rare amongst candidates whose experience of front-end web development has been limited to JavaScript frameworks.

## Additional Information

### Assets

The below assets have been provided to help complete the challenge.

| Name                                          | Description                                                                                      |
|-----------------------------------------------|--------------------------------------------------------------------------------------------------|
| [controls.pdf](assets/controls.pdf)           | Visual design for the controls page feature provided by the Design team                          |
| [documentation.pdf](assets/documentation.pdf) | Visual design for the documentation page feature provided by the Design team                     |
| [controls.json](assets/controls.json)         | Sample controls API response in [JSON:API](https://jsonapi.org/) format provided by the API team |
| [logo.svg](assets/logo.svg)                   | Q-CTRL logo provided by the Brand team                                                           |

## Contributing

See [Contributing](https://github.com/qctrl/.github/blob/master/CONTRIBUTING.md).

## Credits

See [Contributors](https://github.com/qctrl/front-end-challenge/graphs/contributors).

## License

See [LICENSE](LICENSE).
