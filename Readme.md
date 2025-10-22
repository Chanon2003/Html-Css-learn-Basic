ep1
<button>Soi</button>
<p>Seen</p>
<a>Link to yt</a>
<a href="https://www.twitch.tv/" target="_blank">Link to yt1</a>

e2
<style>
  .subscribe-button {
    background-color: rgb(204, 0, 0);
    color: white;
    border: none;
    height: 36px;
    width: 112.992px;
    border-radius: 2px;
    cursor: pointer;
    margin-right: 8px;
  }

  .join-button {
    background-color: white;
    border-color: rgb(41, 118, 211);
    border-style: solid;
    border-width: 1px;
    color: rgb(41, 118, 211);
    height: 36px;
    width: 62px;
    border-radius: 2px;
    cursor: pointer;
  }

  .tweet-button {
    background-color: rgb(2, 158, 255);
    color: white;
    border: none;
    height: 36px;
    width: 70px;
    border-radius: 18px;
    cursor: pointer;
    font-weight: bold;
    font-size: 15px;
    cursor: pointer;
    margin-left: 8px;
  }
</style>

<button class="subscribe-button">SUBSCRIBE</button>
<button class="join-button">JOIN</button>
<button class="tweet-button">twitch</button>
------------------------------------------------------------

ep3
:hover
:activate

opacity:0-1;
transition: opacity 1s;         //แนะนำ 0.15s
transition: background-color 1s,color 1s;
box-shadow: 0 0 0 black;
box-shadow: -10px -10px 10px black;
box-shadow: -10px -10px 10px rgba(0, 0, 0, 0.2);
10px 10px 10px
1.ไปทางขวา
2.ไปด้านล่าง
3.เบลอ 
4.rgba rgb+opacity 0->1
------------------------------------------------------------

ep4
margin
margin-left: 20px;

padding-top: 50px;
padding-right: 30px;
padding-bottom: 50px;
padding-left: 80px;

padding: 25px 50px 75px 100px; t-r-b-l
padding: 25px 50px 75px; //t=25,r,l=50,b=75
padding: 25px 50px; //t,b=25,r,l = 50
padding: 25px; //all = 50

vertical-align: top;


------------------------------------------------------------
ep5 text style

font-family: Arial;
font-size: 30px;
font-weight: bold;
font-style: italic;
text-align: center;
line-height: 20px;  // ความห่าง บรรทัด
ู//html entity middle dot -> &#183;
//checkmarg &#10003;
text-decoration: underline;
<strong></strong> //ตัวใหญ๋
<u></u>  //underline
<span></span>
<p>1<span>2</span><strong>3</strong></p>


------------------------------------------------------------
ep6 the html structure
head{
  <title></title>
  <link rel="stylesheet" href="./buttons.css">
}

------------------------------------------------------------
ep7 image and textbox
ใช้ได้แค่ width ปรับขนาดเมื่อ ปรับ width height ก็จะปรับด้วย

img
height:200px
weight:200px
object-fit: cover; //เอาแค่ขนาดภายใน cover อาจตัดขอบ ใช้กับ
object-position: right;

object-fit: contain;//ก็จะเอาทั้งรูปไปยัดอยู่ใน 200 *200 ให้ได้

.thumbnail{
      width: 300px;
      height: 300px;
      object-fit: contain;
      object-position: top;  //top,bottom,left,right
      border: 1px solid red;
}

<input type="text">
<input type="checkbox">  //ปุ่ม ตื้กถูก

<input type="text" placeholder="Search">

***ใส่ vertical-align: middle; ให้ ทุก inline/inline-block ที่ต้องการเรียงแนวเดียวกัน

------------------------------------------------------------
ep8 css display property

1.block element
=takes up the entire line
<p></p>,<div>

2.inline-block element
only takes up as much space as needed
<input>,<img>

3.inline element
appear within a line of text
<strong></strong>

block->inline-block
display:inline-block;

inline-block -> block;
display:block;

------------------------------------------------------------
ep9 div element

<div> = block

------------------------------------------------------------
ep9 div element
vertical vs horiziontal
v-
1-----
2-----
3-----
h-
1 2 3 
- - -
- - -
- - -
font-family: Roboto, Arail;  //backup dont

------------------------------------------------------------
ep11
display: grid;
grid-template-columns: 100px 100px;

grid-template-columns: 100px 1fr;
column-gap: 20px;
row-gap:20px;

and width:100% in container เช่นรูปที่อยู่ใน

------------------------------------------------------------
ep12
display: flex;
flex-direction: row;  

justify-content: start;    [---      ]
justify-content: end;      [      ---]
justify-content: center;   [   ---   ]
justify-content: space-between;  [-   -   -]

height: 200px;
align-items: stretch; ยืดเต็ม
x
x
x
align-items: start;
x
-
-
align-items: center;   
-
x
-
align-items: enter;
-
-
x   


<div style="background-color: lightblue; width: 100px;">div1</div>
<div style="background-color: lightpink; flex:1">div2</div>
<div style="background-color: lightblue; flex:2">div3</div>

flex diff grid
grid ต้องกำหนดค่ามาก่อนเช่น grid-template-columns: 100px 1fr;
แล้ว div ต้องตรงตพแหน่ง
flex สามารถกำหนดค่าทีหลังไดเช่น display:flex;
width:100px;
flex:1;
flex:2;

max-width: 300px //อาจใช้กับ flex

flex:1;
max-width: 300px;

------------------------------------------------------------
ep13 nested flexbox

box-shadow: inset 1px 2px 5px rgba(0,0,0,0.25);
//inset คือ เงาด้านใน

margin-left: -1px;    1px push,-1px pull

***
flex-shrink: 0;
//no matter what happend, keep this width and we're not going to shrink

width:100px
flex-shrink: 0;

width:0px //shrink

overflow: hidden; //ตัดส่วนเกิน


------------------------------------------------------------
ep14 css position
position: static; คือ ค่าเริ่มต้น (default) ของ position ใน CSS 🧩

position:fixed; //stikcy แค่ถ้าใช้ fixed มันจะทับกับ body ต้องเผื่อระยะ
++top:0px  ติดบน
or top:0;

ต้องใช้ position:fixed;  ก่อน
top:100px ห่างบน100
left:50px;
right:50px;
bottom:50px;
//ถ้าใช้ ซ้ายขวาพร้อมกันมันจะยืดดด


z-index: 0;  // 0-100 ยิ่งสูงยิ่งโชวก่อน แต่ถ้าไม่ใช้ มันจะเรียงตาม code

//overlay จะคุมเพราะ อยู่ข้างล่าง
  <div class="right-sidebar">
    right sidebar
  </div>

  <div class="overlay">
  
  </div>

  
//overlay จะไม่คุมเพราะ อยู่ข้างบน ข้างล่างมาใหม่สูงกว่า
  <div class="overlay">
  
  </div>
  
  <div class="right-sidebar">
    right sidebar
  </div>

//fixed ใช้แค่ div ใหญ่ ครั้งเดียว อย้่าใส่ข้างใน ซ้ำซ้อนไม่งั้นจะทับกันให้ใส่ flex แทน ข่างใน

------------------------------------------------------------
ep15 position absolute and relative

position: absolute;  // แน่นอน
ทำเหมือน fixed เลยสามารถ top:0 bottom:0 l ,r 0;

**
fixed = placed in the browser window
absolute = placed on the page

if posion absolute inside fix it's mean top 0 = top fix


position: relative;  // ญาติ

absolute ต้องตามหลังหรืออยู่ข้างในเสมอ เช่น อยู่ใน fixed,relative

------------------------------------------------------------
ep16 finish project

//อันนี้คือ เฉพาะ class tooltip ทีอยู่ใน search-button เท่านั้น
.search-button .tooltip{
  posintion:absoulte;
}

div class = search-button
  div class = tooltip //ได้

div class = tootip //ไม่ได้ อยู่ด่านนอก

ใส่ 
opacity:0;
แล้วเมื่อ hover ใส่ opacity:1;

//
.profile:hover + .pf2 {
  opacity: 1;
}
.profile คือรูป
.pf2 คือ popup
เครื่องหมาย + หมายถึง “พี่น้องถัดไปโดยตรง” (adjacent sibling selector)

------------------------------------------------------------
ep17 more css features
  
  //เมื่อขนาดหน้าจอ 0-600 จัมี 2 column
  @media(max-width:600px){
      .video-grid{
        grid-template-columns: 1fr 1fr;
      }
  }

 //เมื่อขนาดหน้าจอ อย่างน้อย 1000+ จะมี 4 column
  @media(min-width:1000px){
    .video-grid{
      grid-template-columns: 1fr 1fr 1fr 1fr;
    }
  }

  //combind 1+2 เมื่อขนาด >=751 และ <= 999 จะมี 3 column
  @media(min-width:751px) and (max-width:999px){
    .video-grid{
      grid-template-columns: 1fr 1fr 1fr;
    }
  }


::placeholder ใช้ตกแต่งเฉพาะ ข้อความใน placeholder เท่านั้น

<input type="text" placeholder="กรอกชื่อของคุณ" />


input::placeholder {
  color: gray;
  font-style: italic;
  opacity: 0.7;
}

.search-bar::placeholder{

}
หมายความว่า:
👉 ให้กำหนด “สไตล์ของข้อความ placeholder” สำหรับ input หรือ textarea ที่มี class ชื่อว่า search-bar

<input type="text" class="search-bar" placeholder="ค้นหา..." />

.search-bar::placeholder {
  color: gray;          /* เปลี่ยนสีตัวอักษรของ placeholder */
  font-style: italic;   /* ทำให้ตัวเอียง */
  opacity: 0.8;         /* ทำให้จางลงหน่อย */
}

Semantic Elements (แท็กเชิงความหมาย)
| หมวด                         | Element     | ความหมาย / ใช้สำหรับ                                           |
| ---------------------------- | ----------- | -------------------------------------------------------------- |
| **โครงสร้างหลักของหน้าเว็บ** | `<header>`  | ส่วนหัวของเว็บหรือ section (มักมีโลโก้, เมนูนำทาง)             |
|                              | `<nav>`     | ส่วนเมนูนำทาง (navigation links)                               |
|                              | `<main>`    | ส่วนเนื้อหาหลักของหน้าเว็บ                                     |
|                              | `<section>` | กลุ่มเนื้อหาหลัก ๆ ที่เกี่ยวข้องกัน                            |
|                              | `<article>` | บทความหรือเนื้อหาที่แยกอิสระได้ (เช่น blog post)               |
|                              | `<aside>`   | เนื้อหาข้างเคียง เช่น sidebar, โฆษณา, ลิงก์เพิ่มเติม           |
|                              | `<footer>`  | ส่วนท้ายของหน้าเว็บหรือ section (มักมีลิขสิทธิ์, ข้อมูลติดต่อ) |
