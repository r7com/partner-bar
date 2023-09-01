## 1. Implementation

Follow the steps below to implement the Partner Bar

### Step 1: Include the script in the head of the site

> 1. Open your website's HTML file<br>
> 2. Locate the <head> section of the document<br>
> 3. Copy and paste the code below into the header

```sh
<script id="partners-bar" type="module" src="https://assets.r7.com/cda-partners-bar/cda-partners-bar/cda-partners-bar.esm.js"></script>
```
The script tag should just have the type="module", no need for async and defer. By default the type module already behaves without blocking the rendering of the page and implicitly there is already a "defer" mode when using the type module, and therefore, the script can stay in HTML. It is important to remove lazy load scripts, cache and other plugins inside the bar to avoid performance problems because the browser itself will cache the script after the first request.

---
### Step 2: Insert the attributes in the <body> of your website
    
> 1. Locate the <body> section of the document<br>
> 2. Copy and paste the code below and make sure it is the first element right after the opening tag

```sh
<cda-partners-bar tag-manager="true" record-origin-only="true" no-follow='true'></cda-partners-bar>
```
---

## 2. Verification

After the implementation is complete, follow these steps to verify that the New Partner Bar is working correctly:

> 1. Open your website in a browser<br>
> 2. Make sure the New Partner Bar is displayed correctly at the top of the site<br>
> 3. Test bar functionality such as link clicks and interactions
---

## 3. Attributes

| Attribute                               | Description                                                                                 |
| --------------------------------------- | ------------------------------------------------------------------------------------------- |
| `record-origin-only`                    | Enables the option to display the bar only when the user accesses the site through R7.      |
| `tag-manager`                           | Enables tagManager                                                                          |
| `no-follow`                             | Enables no-follow in the itens of menu                                                      |

