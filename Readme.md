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