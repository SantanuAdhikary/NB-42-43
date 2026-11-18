
# HTML 

**what is HTML**

* `HTML` stands for **Hypertext Markup Language**, it is used to create the structure of webpage.


**why it is called Markup Language ??**

* html is not programming language because here we are not writing any logics , here we are creating structure of webpage by using tags.

**what is hyperText**

* any text that contains link of any other webpage is called as `hyperText`


## Structure Of HTML 

<!DOCTYPE html>
<html>
    <head>
        
        <title>  </title>
    </head>

    <body>
        
    </body>
</html>


**<html></html>**

 * this is the `root tag` in html document.
 * whatever code we will write everything should be inside this tag.

**<head></head>**
 
 * this tag is used to provide the information about the document.

**<title></title>**
 
 * it is used to provide the name of the document.
 * in browser this name will be displayed in the tab.

 **<meta>**

 * this is used to provide some additional information like which character-set we are writing the code, which size device can display our code.

 **<body></body>**

 * this tag is used to display all the tags content on the UI.
 * we have to write all the html tags inside `body tag`.

 **<!DOCTYPE html>**

  * it is used to tell the version of html.
  * currently we are using html5

## Tags 

* tags are predefined words enclosed with angular braces <>
* there are 2 types of tags. 

1. Paired Tag 
2. Unpaired Tag / Self closing tag


### 1. Paired Tag 

* here we have both opening and closing tag.

    <tagname> </tagname>

eg:  h1, p , b , body 

### 2. Unpaierd / Self closing Tag

* these tags have only the opening tag, there is no closing tag.

    <tagname>

eg:   br , hr , meta

## Formatting Tags

* these tags are used to change the appearence / format of the text.


**<b></b>**
  * this tag is used to make the text bold. 

eg:
    <p> my name is <b>santanu </b> </p>

**<strong></strong>**

 * this tag is also used to make the text bold.
 * this tag having the higher priority in browser compare to b tag.

**<u></u>**

 * used to provide underline.

**<ins></ins>**
 
 * this tag is also used to provide underline.

**<i></i>**
 
 * used to make the text italic.

**<em></em>**

 * it is also used to make the text italic.

**<mark></mark>**

 * this tag is used to provide highlight to the text.

 **<q></q>**

 * this tag is used to provide double quotes around the text.

 **<sup></sup>**

 * this tag is used to write any text content to the power of any other text.

 eg: 
       <p>1 <sup>st </sup> <p>

**<sub></sub>**

 * this tag is used to write any text content to the base of another text.

**<del></del>**
 
 * it is used to provide strike to the text.

**<strike></strike>**

 * this tag is also used to provide strike but this tag is deprecated.

**<pre></pre>**

* this is called pre formatted tag.
* inside this tag how we will write the content it will display as it is.
* here the font-family will be monospace.


## Heading tags 

* heading tags are used to provide the headline in our webpage. 
* we have total 6 heading tags. (h1,h2,h3,h4,h5,h6)
* the difference between them is size.
* h1 having the largest size and h6 having the smallest size.
* h1 --> 32px 

## Paragraph Tag

* this tag is defined by <p></p>, it is used to write any text content in html.

* the size of this tag is 16px.



## Element 

* element is a combination of tags and the content.

    <tagname> content </tagname>

* in html there are 3 types of element. 

**1. inline level element**
**2. block level element**
**3. inline block level element**


### inline level element 

* these elements will be displaying in the same line. 
* here we can't provide height and width.
* it will occupy only the content area.

eg:   i,b,u tags

### block level element 

* these elements will be displaying in the next line. 
* here we can provide height and width. 
* it will occupy full width of its parent element.

eg: all heading tags, p tag, div, section

### inline block level element 

* these elements are combination of both inline and block level element.
* these elements diplay in same line but we can provide height and width.

eg: button,input



## Attributes 

* attributes are used to provide additional / extra information to the tags.

* we should write the attributes in the opening tag.

*syntax*
   
   <tagname attributename = "value" > </tagname>


## <img> tag

* this tag is used to add image in our webpage.

**attributes**

*src*
   * this is used to give the path of the image.

*alt*
   * this is used to provide alternate message.
   * if the image is not loading that time this message will be displayed.

*height and width*
   * these attributes are used to resize the image.


## <marquee></marquee> tag


* this tag is used to scroll content on the webpage.

* by default the content will scroll from right to left.

### attributes 

**direction**
  * it is used to define the direction of the scrolling content.
    values are => up / down / right / left 

**scrollamount**   
  * used to increase / decrease the speed. 
  * by default value is `6`.

**behavior**
  * here we can give the values as `scroll`, `alternate` and `slide`.

**loop**
  * by using this we can define how many times the content should scroll.

**height and width**
  * used to resize the tag. 

```html
  
    <marquee behavior="alternate" direction="right" scrollamount="30">

          <h1> hello everyone</h1>
    </marquee>
    
```

## List In HTML 

* it is the process of grouping the related elements together.
* in html we have 3 types of list.

**1. Ordered List**
**2. Unordered List**
**3. Description List**


### ordered list

* here all the elements will be organized in particular order.
* we have to create ordered list by using <ol> </ol> tag. 
* inside that elements will be created by using <li> </li> tag.

#### attributes

 **type**
    
  * this attribute is used to define the list style.
  * by default value will be number.
  * we can provide the value as `a` / `A` / `i` / `I` / 1

 **start**
  
  * it is used to specify the starting value of the list-style.

 **reversed**
  
  * it is used to display the list-style in reverse order.


```html


  <ol type="a" start="5" reversed>
      <li> sql</li>
      <li> java</li>
      <li> python</li>
  </ol>

```
```output
 e. sql
 d. java 
 c. python
```


E  J   O   T   Y 

5 10   15  20  25


### Unordered List 

* unordered list we can create by using <ul> </ul> tag
* inside that we have to give <li></li> tag.
* when we are creating this, by default it will give bullet points.

#### attributes

**type**
  
  * by default value is `disc`.
  * we can give `square`, `circle`, `none`

```html
  
  <ul type="circle">
     <li> mt </li>
     <li> at </li>
     <li> react </li>
  </ul>

```

### Description List 

* this list we can create by using <dl> </dl> tag

* inside this we can give <dt></dt> tag to provide the **description term**

* we hav <dd></dd> tag , it is called as **description definition**, used to provide some information about the term.

```html

 <dl>
    <dt> HTML </dt>
    <dd> stands for hypertext markup language, used to create structure of webpage </dd>
 </dl>


```

## HyperLink 

* any content if that contains link of any other webpage is called `hyperlink`.

* we can create hyperlink by using `anchor tag`

### what is anchor tag

* anchor tag is defined by <a></a>

* it is used to navigate from one page to another page or in the same page one section to another section.

* it is *inline-block level* element.

#### attributes 

**href**
 
 * here we have to provide the path of the page where we want to navigate.

**target**
  
  * by default value is ` _self`, it will open in the same tab. 
  * if we want open one new tab then we have to give the value as `_blank`

**title**
 
 * it will display one message when we will keep our mouse cursor on the hyperlink.

 * that message we can define inside this title attribute.


```html

  <a href="https://www.facebook.com" target="_blank" title="fb"> 
    go to facebook
  </a>

```


## what is <br> tag

* this tag is used to break the line, so that content will display in the next line.

## what is <hr> tag

* it is used to create horizontal line.

```html

    <p>  hello everyone <br> how are you ? </p>
    <hr>
```


## iframe tag 

* this tag is used to add different webpage in our current webpage.

### attributes 

**src**
  * it is used to provide the path of the webpage.


**frameborder** 
 
 * this is used to provide outline / border around the content. 

 * by default value is `0`


**height , width**

   * used to resize the content.

* `iframe` tag is **inline block level element.**

* we can add `youtube video` , `google map` by using this tag.

**note**
  * for adding youtube video and map we should use `embed link`


## <audio></audio> tag

* it is used to add any audio file in our webpage.

### attributes

**src**

  * used to provide the path of the audio file.

**controls**

  * without this attribute audio will not be visible on the webpage.

  * if we provide this attribute, audio will display on the webpage and we can play/pause/skip the audio.

**loop**

 * it helps the audio to play repeatedly in a loop.

**autoplay**

 * if we provide this attribute our audio will start playing whenever our webpage will reload.


**muted**
  
  * it will make the audio mute by-default.


## <video></video> tag

* this tag is used to add video on the webpage.

### attributes
   
  * src , controls , loop , muted, autoplay these attributes are same as audio tag.

  **height , width**
    
    * used to resize the video.

  **poster**
    
    * used to provide image for the video.


## table 

* table is a combination of rows and columns. 

* in html for creating table we need <table></table> tag.

* inside table for creating rows we need <tr></tr> tag.

* inside rows we have to give data, for that we can use <th></th> and <td></td> tag.

* to provide the title of the table we can give <caption></caption> tag.

### attributes 

**border**
   * used to provide outline around the table.

**height,width**
   * used to resize the table.

**cellspacing**
   * used to provide space between the cells (outside of the cell)

**cellpadding**
  * used to provide space inside the cell between the content and border.


### attributes of td and th tag

**rowspan**

 * it is used to combine two or more than two rows.

**colspan**

 * it is used to combine two or more than two columns.


* in table we have some more tags like 
 <thead></thead>
 <tbody></tbody>
 <tfoot></tfoot>
 
 * they are semantic tags.