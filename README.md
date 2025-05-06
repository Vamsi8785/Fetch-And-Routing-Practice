In this project, let's perform **Fetch and Routing**.

### Refer to the image below:

<br/>
<div style="text-align: center;">
    <img src="https://assets.ccbp.in/frontend/content/react-js/fetch-and-routing-practice-output.gif" alt="fetch and routing practice desktop output" style="max-width:70%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12)">
</div>
<br/>

### Design Files

<details>
<summary>Click to view</summary>

- [Extra Small (Size < 576px) and Small (Size >= 576px)](https://assets.ccbp.in/frontend/content/react-js/fetch-and-routing-practice-sm-outputs.png)
- [Medium (Size >= 768px), Large (Size >= 992px) and Extra Large (Size >= 1200px) - Home](https://assets.ccbp.in/frontend/content/react-js/fetch-and-routing-practice-lg-blog-list-output.png)
- [Medium (Size >= 768px), Large (Size >= 992px) and Extra Large (Size >= 1200px) - Blog Item Details](https://assets.ccbp.in/frontend/content/react-js/fetch-and-routing-practice-lg-blog-item-output.png)

</details>

### Set Up Instructions

<details>
<summary>Click to view</summary>

- Download dependencies by running `npm install`
- Start up the app using `npm start`
</details>

### Completion Instructions

<details>

<summary>API Requests & Responses</summary>
<br/>

**blogsApiUrl**

#### API: `https://apis.ccbp.in/blogs`

#### Method: `GET`

#### Description:

Returns a response containing the list of all blogs

#### Response

```json
[
  {
    "id": 1,
    "title": "React v16.9.0 and the Roadmap Update",
    "image_url": "https://miro.medium.com/max/1050/1*i3hzpSEiEEMTuWIYviYweQ.png",
    "avatar_url": "https://miro.medium.com/max/4096/1*wiOSfPd2sY0gXSNK9vv6bg.jpeg",
    "author": "Dan Abramov,",
    "topic": "React.js"
  },
  ...
]
```

**blogItemDetailsApiUrl**

#### API: `https://apis.ccbp.in/blogs/:id`

#### Example: `https://apis.ccbp.in/blogs/2`

#### Method: `GET`

#### Description:

Returns a response containing the details of the specific blog

#### Response

```json
{
  "id": 2,
  "title": "React v16.7: No, This Is Not the One With Hooks",
  "image_url": "https://miro.medium.com/max/3158/1*kEPCQNY4dwVyaFuLEwJcNQ.png",
  "avatar_url": "https://avatars.githubusercontent.com/u/3624098?v=4",
  "author": "Andrew Clark",
  "content": "React follows semantic versioning. Typically, this means that we use patch versions for bugfixes, and minors for new (non-breaking) features. However, we reserve the option to release minor versions even if they do not include new features. The motivation is to reserve patches for changes that have a very low chance of breaking. Patches are the most important type of release because they sometimes contain critical bugfixes.",
  "topic": "React.js"
}
```

</details>

<details>
<summary>Components Structure</summary>

<br/>
<div style="text-align: center;">
    <img src="https://assets.ccbp.in/frontend/content/react-js/fetch-and-routing-practice-home-component-breakdown-structure.png" alt="fetch and routing practice home component breakdown structure" style="max-width:100%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12)">
</div>
<br/>
<div style="text-align: center;">
    <img src="https://assets.ccbp.in/frontend/content/react-js/fetch-and-routing-practice-blog-item-component-breakdown-structure.png" alt="fetch and routing practice blog item component breakdown structure" style="max-width:100%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12)">
</div>
<br/>
</details>



> ### _Things to Keep in Mind_
>
> - All components you implement should go in the `src/components` directory.
> - Don't change the component folder names as those are the files being imported into the tests.
> - **Do not remove the pre-filled code**
> - Want to quickly review some of the concepts you’ve been learning? Take a look at the Cheat Sheets.
