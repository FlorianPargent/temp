This repository will be used whenever I want to quickly host a Quarto website at:  
<https://florianpargent.github.io/temp/>

### **WARNING: All hosted content is extremely temporary. Everything can change or be removed at any time!**

---

*Instructions to myself:*

- Place .qmd file in the temp/ project folder
- Make sure to use the following yaml options:  
```
format:
  html:
    embed-resources: true
```
- Publish website with the following command:
```
quarto publish gh-pages document.qmd
```

- You can use [quarto-webr](https://github.com/coatless/quarto-webr) to include code cells that run R in the browser:
    - install quarto extension:
    ```
    quarto add coatless/quarto-webr
    ```
    - add webr to the yaml header of the .qmd document:
    ```
    filters:
      - webr
    ```
    - add webr code chunks to .qmd document:
    ```
      ```{webr}
      ```
    ```
    - it seems like `embed-resources: true` destroys the webr html buttons
