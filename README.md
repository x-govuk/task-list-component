# task-list-component

## Installation

[Set up the GOV.UK Prototype Kit in the usual way](https://govuk-prototype-kit.herokuapp.com/docs/install) then install the task list component using:

`npm install --save git@github.com:x-govuk/task-list-component.git#v0.0.1`

You can then start the kit as usual with `npm start`

## Usage example

Once you've installed it try adding this snippet to one of your views:

```
{% from "task-list-component/macro.njk" import govukTaskList %}
{{govukTaskList({
  items: [
    {
      href: "https://google.com/",
      hint: {text: "Google is good"},
      title: {text: "Google something"},
      statusId: "ggl",
      status: {
        classes: "govuk-task-list__status--light-blue",
        text: "In progress"
      }
    },
    {
      href: "https://bing.com/",
      hint: {text: "Bing is bad"},
      title: {text: "Bing something"},
      statusId: "bng",
      status: {
        classes: "govuk-task-list__status--error",
        text: "I refuse"
      }
    }
  ] 
})}}
```

Any questions, comments etc. please raise an issue.
