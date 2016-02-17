# expand-collapse-box2
MA interactive journo class expand collapse box
<H1> for in this scenario stands for heading one always within crab hands in HTML
If there are more heading it is recommended you number them “h2, h3” etc.

<h1>
Article
</h1>

<P> stand for paragraph and this is where the body of the article should go.
If you have multiple paragraphs you should have multiple P’s.

<p>
Lorem ipsum dolor sit amet, idque utroque id eum, has erant periculis ad, delenit laboramus his ei. Ne agam dicam eum, est quodsi deterruisset ne. Ut mea movet oporteat constituam, summo argumentum id nec.
</p>

<div> is a box but I’ve assigned a class to it because i have some CSS work to go along with it. 
I chose to use the “more-less-box> but you can name it whatever you want.

<div class="more-less-box">

<h3> There is also another heading inside the box that is going to expand, which is why I have a heading 3.
<h3>
Fact box
</h3>

I have given P a class here to because again I’m going to add some CSS to make the box expand and collapse with the text inside.
<p class= "more-less-area collapsed">
Lorem ipsum dolor sit amet, idque utroque id eum, has erant periculis ad, delenit laboramus his ei. Ne agam dicam eum, est quodsi deterruisset ne. Ut mea movet oporteat constituam, summo argumentum id nec.
</p>

<A> is used to build links and I have added a class to it because I’m going to add some CSS to the button that is going to toggle. 

Href stankds for the link and javascript:void(0) is telling jsfiddle not to move the button unless its clicked on or “onclick”

toggleMoreLess('.more-less-area')"> is telling jsfiddle to toggle the more-less-are.

<a class="more-less-button"
href="javascript:void(0);" onclick="toggleMoreLess('.more-less-area')">Show/Hide Box</a>
</div>


P is my lest and final paragraph. 

<p>
Lorem ipsum dolor sit amet, idque utroque id eum, has erant periculis ad, delenit laboramus his ei. Ne agam dicam eum, est quodsi deterruisset ne. Ut mea movet oporteat constituam, summo argumentum id nec.
</p>

CSS

We start off with .collapse because that is the class we assignment for in HTML and where we want jsfiddle to work.

We assign and maximum height to the box that contains the text and the more-less-area.
We also assign a overflow that is going to be hidden.
The CSS is where you can get creative in design so you are welcomed to do more.

.collapsed{
  max-height: 20px;
  overflow: hidden;
}

We start off with .more-less-ares because that is the class we assignment for in HTML and where we want jsfiddle to work.

Float: left means that the box is going to float to the left.

background: #99ffff; is the tortoise colour I choose for the background but you can choose any colour.

border-radius: 10px; is the border that I have assigned for in 10px, but you can choose your our border.

Margin is a margin and I choose 20px.

Padding is padding and I choose 20px.

.more-less-box{
  float: left;
  background: #99ffff;
  border-radius: 10px;
  margin: 20px;
  padding: 20px;
}

JAVA

The JAVA is really key to make the more or less area toggle and close.

We assigned a function to toggle the more or less areaClass

function toggleMoreLess(areaClass) {
$(areaClass).toggleClass('collapsed');
}
