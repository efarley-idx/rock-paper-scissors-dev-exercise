# IDX UX Applicant Exercise

### Hello and welcome!

We here at IDX have designed this development exercise in order for us to get a better idea on your code style, approach to problem solving as well as how you complete development tasks. We will use the code you provide to help inform us about your coding and if you're selected for an interview, we will review your code sample as a group. While there is no right or wrong approach to this excercise you should be prepared to discuss your code and answer questions about how you approached the problem, what parts you enjoyed writing, what parts were difficult for you and why you did or did not make certain decisions.

## Your task, should you choose to accept it...

You have a fairly simple task, develop a game which you're probably already familiar with; Rock Paper Scissors. However, while at its core that should be a simple task, we'll add some acceptance criteria (AC) to help you showcase the particular skills that we're looking for from our applicants. In addition to the AC you're more than welcome to add whatever flair or personal touch you are compelled to add. You might even find an easter egg if you're astute ;)

## Acceptance Criteria

- **As a** User **I want** to understand the core rules of the game. I.e. Rock smashes Scissors. **So that** I can play the game without confusion.
- **As a** User **I want** to have a simple user interface that allows me to select my gesture, see my opponents gesture and review the results. **So that** I can play the game with my mouse.
- **As a** Developer **I want** to have confidence future changes will not cause a regression in my code using unit testing **So that** I can easily maintain the application.
- **As a** Developer **I want** to maintain the state of the application using _NgRx_ **So that** I have a single source of truth for the applications state.
- **As a** Developer **I want** to consume API endpoints to get the available Gestures and get the opponents Gesture **So that** I don't have to define the application data or calculate opponent gestures.
- **As a** QA Tester **I want** to be able to run automated tests using Protractor to verify the application works as expected **So that** I can quickly check pull requests for regressions.
- **As an** Applicant **I want** to use _Angular_ **So that** I can be fairly evaluated against my competition.

## Code Formatting

- **Do** use 2 space tabs.
- **Do** type all variables.
- **Do** use observables over promises.

## API Endpoints

`GET` `https://idx-ux-dev-test.herokuapp.com/gestures`

Response:

    enum Gestures {
      Rock,
      Paper,
      Scissors
    }

`GET` `https://idx-ux-dev-test.herokuapp.com/opponents-gesture`

Response:

    {
      gesture: Gestures
    }

## Resources

**How to play?** _Rock_ beats _Scissors_, _Scissors_ beats _Paper_, and _Paper_ beats _Rock_.

**Boilerplate** This repo is set up with a pre generated _Angular 10_ application using _Angular Material_, _Flex Layout_, and _NgRx_, feel free to use these resources as needed.

**Design** We have provided you with a simple design to follow and the necessary resources to implement it since we know that not everyone likes doing UX design. However, if you're inclined feel free to add your own flair to the design, or blow us away with something unique.

Assets can be found in the directory `/src/app/assets/images`

![Design Mockup](https://dl.boxcloud.com/api/2.0/internal_files/732253759462/versions/779514690262/representations/png_paged_2048x2048/content/1.png?access_token=1!x3wMYP7RX8CXrYc4ugmvmceJVGyM69NoxkARPMh2vRNYXk5CnyKyKFKnonf95xwRB4s_afrDgKQNHbbrqCkLcFL8qfy-usMYKO9kgWVTx766624ybaa_EMWEn1JYitRN8zHOAcq-JvPuj7ugfrNuJ_pddocF46WXmVne4j21rfQfD1NgHqjyxH4BRhXw-MVbOwKtE31MPBr8X9YBh6f2SbUgcfVoV2bdo7c1QLJXiNEAmPmH-S-aSKdPiJDm68waGCx26N5y6VOuqtVuUhVlyiY8iD-gpiYerk6dXxnzQWBv7XiWcQluFmcRNQTumwNSABDmwer2WmH_uk1Jo_4mQv5jiPIWXi2-JhUiiYjkQ6GSc3ZkBkJjP9u-RLM8J5R1A6yA4tNSRW_SpHfEnIyW0T5t2fIi3vho1osMwOkNfaYxRzo6YBWN33h8X1jc_SkzQttEPtNUdLkVFlCm90TCQn7sAxCnrb2nG4YuWr6VQlGmxkmpkAyjDNXRtXRDAkTqVT7kLzKlZLwZXwANhIsyTc5h_5l6G-mO881yVZaSRuuQJRI-ZSfxGXnJEwrRY5kyTlBxKnNZxzyeOCtkejf62SphtuOldCPwTTvRldBadfdO4CUE7NAlNvov__TiM5WGwL3zhR4hG87tMvQYwU_UXQns-f79ET2oF5AWUPJKnT7DzBJA&box_client_name=box-content-preview&box_client_version=2.52.0)

### Branding 

**Body**

    color: black;
    font-family: Roboto, "Helvetica Neue";
    font-size: 1em;

**Heading**

    font-size: 3em;
    font-weight: 100;

**Sub-heading**

    color: rgba(0, 0, 0, .65);

**Ready button**

    background-color: #673ab7;
    color: white;

**Unselected gesture image**

    background-color: #aeabb0;
    border-radius: 100px;
    height: 200px;
    width: 200px;

**Selected gesture image**

    background-color: #673ab7;

**Gesture name**

    color: rgba(0, 0, 0, .65);
    font-size: 1.75em;
    font-weight: 100;
    margin-top: 10px;

## Where to start

1. Clone the repository to your local machine.
1. Run the command `npm install`.
1. Begin making your changes.

## How to submit your code

In order to submit your code follow these steps.

1. Ensure that `ng serve` serves your application without errors.
1. Ensure that `ng test` runs your unit tests.
1. Ensure that `ng e2e` runs your e2e tests.
1. Delete the `./node_modules` directory.
1. Zip the `root` directory.
1. E-mail the `.zip` file to matt.mcguire@idexpertscorp.com and eric.farley@idexpertscorp.com.