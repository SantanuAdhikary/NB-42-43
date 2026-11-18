
# CSS 

## CSS Introduction

* CSS stands for `Cascading Style Sheets`
* it is used to provide style to our webpage and it is used to arrange all the elements what we have created by using html.

### How many ways we can write css ? 

* we can write css in 3 ways. 

**1. Inline CSS**
**2. Internal CSS**
**3. External CSS**

### Inline CSS 

* this is the process of writing the css inside the tag itself.
* for this we need `style` attribute.

```html

    <p style="color:red; text-align:center"> my name is santanu</p>

```


### Internal CSS

* this is the process of writing the css code inside the same html file.

* for this we need <style></style> tag, and this tag we should write inside <head></head> tag.

### External CSS 

* this is the process of writing css code in separate css file.

* we have to link between the html and css file by using <link> tag.

* in <link> tag we have to give the path of the css file inside the `href` attribute.


**Note**

 * between this three , `inline css` having the higher priority.

 * between `internal` and `external` both having the same priority.
   which one is coming at the end will be applied.



## Selectors In CSS

* selectors are used to select the html element to apply the css.

* we have 5 types of selectors in css. 

**1. Simple Selector**
**2. Combinator Selector**
**3. Pseudo Class Selector**
**4. Pseudo Element Selector**
**5. Attribute Selector**


### Simple Selector 

**1. tagname selector**

  * by using this selector we can select any html element by their tagname.

  * it will target all the elements who having the same name.

**2. Id selector**

 * if we want to target any element individually then we can use this selector.

 * we have to provide `id` attribute inside the tag then from css we have to target by the same id name and for that we have use `#` symbol.

 * we should not provide same id to more than one element.

 **3. class selector**

  * if we want to apply same css to more than one element we have to use this selector.

  * to apply this selector,inside tag we should use `class` attribute and from the css we have to target by using `.classname` 

**4. universal selector**

  * by using this selector we can target all the elements that is present in our html page.

  * by using `*` symbol we can apply this selector.

**5. Group Selector**

 * by using this selector we can group more than one selectors.

 * to apply this we have to use `,` symbol.



 #### syntax of selector

    selector{
        property1 : value ; 
        property2 : value ; 
        property3 : value ; 
      
    }

### Combinator Selector 

* it is the combination of two or more than two simple selectors.

*types*

**1. Descendant Selector**
**2. Direct Child Selector** 
**3. Adjacent Sibling Selector** 
**4. General Sibling Selector**

#### Descendant Selector 

* by using this selector we can target child,grand child,great grand child element.

* for applying this we have to provide space b/w the selectors.

#### Direct Child Selector 

* this selector will target only the child directly related to the parent element.

* to apply this we have to use `>` symbol b/w the selectors.

#### Adjacent Sibling Selector

* this selector will select the next element.
* both elements parent should be same.
* here we have to use `+` symbol.

#### General Sibling Selector 

* this selector is defined by `~` symbol.
* it will target all the next sibling element.


### Pseudo Class Selector

* `Pseudo class selector` we can apply by using `:` symbol.

**Types**

#### 1. hover

 * when we will keep our mouse cursor on the element that time this selector will change the css.

 #### 2. active

 * when we will click on the element that time itt will apply this selector's css.

 #### 3. nth-child

   * it is used to target any element by the child number.

   * we can target all the odd and even elements also by using this selector. 

   ```css

      ul > li:nth-child(2n)
      {
           // it will target all the even list
      }

      ul > li:nth-child(2n + 1)
      {
           // it will target all the odd list
      }

   ```
  #### 4. first-child and last-child

  * these selectors are used to target the first and last child of any element.

  #### 5. focus 

  * when we are focusing on any input or text-area that time we can use this selector to change the css.


### Pseudo Element Selector 

* for applying this selector we have to use double colons ` :: `

#### 1. first-letter

 * it is used to target the first letter of any text content. 

 ```css
      .hero p::first-letter{
          font-size: 40px;
      }
 ```

 #### 2. first-line 

  * it is used to target the first line of any text content.

#### 3. selection 

  * when we are selecting any content on the webpage, that time if we want apply some css we can use this selector.

#### 4. before and after 

 * these selectors are used to add content from css before and after the selected element.

 **Note** we should use `content` key here.

 ```css
         .hero > h1::after{
           content : "***",
           color : red
         }
 ```

#### 5. marker

 * it is used to target the list style.

#### 6. placeholder 

* used to target the placeholder inside input or text-area tag.


## Attribute Selector 

* by using this selector we can target the element by their attributes.

*syntax*
 
   tagname[attributename = "value"]
   {
    
   }





   positoion absolute will change the position of the element based on the nearest ancestor.