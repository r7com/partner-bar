## 1. Implementation

Follow the steps below to implement the Partner Bar

### Step 1: Include the script in the head of the site

> 1. Open your website's HTML file<br>
> 2. Locate the <head> section of the document<br>
> 3. Copy and paste the code below into the header

```sh
<script async defer id="partners-bar" type="module" src="https://assets.r7.com/cda-partners-bar/cda-partners-bar/cda-partners-bar.esm.js"></script>
```

### Step 2: Insert the attributes in the <body> of your website
    
> 1. Locate the <body> section of the document<br>
> 2. Copy and paste the code below and make sure it is the first element right after the opening tag

```sh
<cda-partners-bar style="height: 50px;display: block;" tag-manager="true" record-origin-only="true" no-follow='true'></cda-partners-bar>
```
---

## 2. Verification

After the implementation is complete, follow these steps to verify that the New Partner Bar is working correctly:

> 1. Open your website in a browser<br>
> 2. Make sure the New Partner Bar is displayed correctly at the top of the site<br>
> 3. Test bar functionality such as link clicks and interactions
---

## 3. Hint for Attaching the Bar
```sh
   .cda-container
     visibility: hidden;
     position: fixed;
     top: 0;
     left:0;
     width: 100%;
     display: flex;
     justify-content: center;
     align-items: center;
     min-height: 50px;
```
---

## 4. Attributes

| Attribute                               | Description                                                                                 |
| --------------------------------------- | ------------------------------------------------------------------------------------------- |
| `record-origin-only`                    | Enables the option to display the bar only when the user accesses the site through R7.      |
| `tag-manager`                           | Enables tagManager                                                                          |
| `no-follow`                             | Enables no-follow in the itens of menu                                                      |
| `style="height: 50px;display: block;"`  | Adds a 50px space to the slash thus preventing CLS error (optional)                         |

