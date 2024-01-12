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
