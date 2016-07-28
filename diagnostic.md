# Ember Components Diagnostic

Record your responses inside the fenced code blocks below each question.

1.  Give an example of a visual hierarchy that could be modeled with components.

    ```md
    A contacts book with indiviudal 'contact cards' that hold data about the
    contact.
    ```

1.  What is the command to generate a new component called '`my-map`'?

    ```sh
    ember generate component my-map
    ```

1.  What files are edited to produce a component, and what are their
    responsibilities?

    ```md
    The two files in a component's directory are component.js & template.hbs.
    Template holds markup that determines what will be rendered by the component
    and the Javascript file holds the 'component object' which includes all of
    the behaviors of the component (actions, class bindings, etc)
    ```

1.  Suppose you have a component '`my-contact`', which is loaded from
    '`app/contacts/template.hbs`' when visiting the `/contacts` path. What is
    the syntax for loading this component inside that template?

    ```html
    {{my-contact contact=contact}}
    ```

    Each contact has multiple phone numbers. Suppose you also have '`my-phone`'
    nested under '`my-contact`'. What is the code you would write in
    '`app/components/my-contact/template.hbs`' to load the nested component and
    pass it data?

    ```html
    {{my-contact/my-phone contact=contact}}
    ```
