




<style>
  @import "rouge-base16-dark";
@import "default_colors";

$body-background: $cod-grey !default;
$body-foreground: $gallery !default;
$header: $conifer !default;
$blockquote-color: $silver-chalice !default;
$blockquote-border: $dove-grey !default;
$container-max-width: 1000px;

@mixin media-max-width($max-width) {
  @media (max-width: $max-width) {
      @content;
  }
}

body {
  margin: 0;
  padding: 0;
  background: $body-background url("../images/bkg.png") 0 0;
  color: $body-foreground;
  font-size: 16px;
  line-height: 1.5;
  font-family: Monaco, "Bitstream Vera Sans Mono", "Lucida Console", Terminal, monospace;
}

/* General & 'Reset' Stuff */

.container {
  width: 90%;
  max-width: $container-max-width;
  margin: 0 auto;
}

section {
  display: block;
  margin: 0 0 20px 0;
}

h1, h2, h3, h4, h5, h6 {
  margin: 0 0 20px;
}

li {
  line-height: 1.4 ;
}

/* Header, <header>
   header   - container
   h1       - project name
   h2       - project description
*/

header {
  background: rgba(0, 0, 0, 0.1);
  width: 100%;
  border-bottom: 1px dashed $conifer; //header;
  padding: 20px 0;
  margin: 0 0 40px 0;
}

header h1 {
  font-size: 30px;
  line-height: 1.5;
  margin: 0 0 0 -40px;
  font-weight: bold;
  font-family: Monaco, "Bitstream Vera Sans Mono", "Lucida Console", Terminal, monospace;
  color: $conifer;//$header;
  text-shadow: 0 1px 1px rgba(0, 0, 0, 0.1),
               0 0 5px rgba(181, 232, 83, 0.1),
               0 0 10px rgba(181, 232, 83, 0.1);
  letter-spacing: -1px;
  -webkit-font-smoothing: antialiased;
  @include media-max-width($container-max-width) {
    margin-left: 0;
  }
}


header h1:before {
  content: "./ ";
  font-size: 24px;
}

header h2 {
  font-size: 18px;
  font-weight: 300;
  color: #666;
}

#downloads .btn {
  display: inline-block;
  text-align: center;
  margin: 0;
}

/* Main Content
*/

#main_content {
  width: 100%;
  -webkit-font-smoothing: antialiased;
}
section img {
  max-width: 100%
}

h1, h2, h3, h4, h5, h6 {
  font-weight: normal;
  font-family: Monaco, "Bitstream Vera Sans Mono", "Lucida Console", Terminal, monospace;
  color: $header;
  letter-spacing: -0.03em;
  text-shadow: 0 1px 1px rgba(0, 0, 0, 0.1),
               0 0 5px rgba(181, 232, 83, 0.1),
               0 0 10px rgba(181, 232, 83, 0.1);
}

#main_content h1 {
  font-size: 30px;
}

#main_content h2 {
  font-size: 24px;
}

#main_content h3 {
  font-size: 18px;
}

#main_content h4 {
  font-size: 14px;
}

#main_content h5 {
  font-size: 12px;
  text-transform: uppercase;
  margin: 0 0 5px 0;
}

#main_content h6 {
  font-size: 12px;
  text-transform: uppercase;
  color: #999;
  margin: 0 0 5px 0;
}

dt {
  font-style: italic;
  font-weight: bold;
}

ul li {
  list-style-image:url('../images/bullet.png');
}

blockquote {
  color: $blockquote-color;
  padding-left: 10px;
  border-left: 1px dotted $blockquote-border;
}

pre {
  background: rgba(0, 0, 0, 0.9);
  border: 1px solid rgba(255, 255, 255, 0.15);
  padding: 10px;
  font-size: 16px;
  color: #b5e853;
  border-radius: 2px;
  word-wrap: normal;
  overflow: auto;
  overflow-y: hidden;
}

code.highlighter-rouge {
  background: rgba(0,0,0,0.9);
  border: 1px solid rgba(255, 255, 255, 0.15);
  padding: 0px 3px;
  margin: 0px -3px;
  color: #aa759f;
  border-radius: 2px;
}

table {
  width: 100%;
  margin: 0 0 20px 0;
}

th {
  text-align: left;
  border-bottom: 1px dashed #b5e853;
  padding: 5px 10px;
}

td {
  padding: 5px 10px;
}

hr {
  height: 0;
  border: 0;
  border-bottom: 1px dashed #b5e853;
  color: #b5e853;
}

/* Buttons
*/

.btn {
  display: inline-block;
  background: -webkit-linear-gradient(top, rgba(40, 40, 40, 0.3), rgba(35, 35, 35, 0.3) 50%, rgba(10, 10, 10, 0.3) 50%, rgba(0, 0, 0, 0.3));
  padding: 8px 18px;
  border-radius: 50px;
  border: 2px solid rgba(0, 0, 0, 0.7);
  border-bottom: 2px solid rgba(0, 0, 0, 0.7);
  border-top: 2px solid rgba(0, 0, 0, 1);
  color: rgba(255, 255, 255, 0.8);
  font-family: Helvetica, Arial, sans-serif;
  font-weight: bold;
  font-size: 13px;
  text-decoration: none;
  text-shadow: 0 -1px 0 rgba(0, 0, 0, 0.75);
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.05);
}

.btn:hover {
  background: -webkit-linear-gradient(top, rgba(40, 40, 40, 0.6), rgba(35, 35, 35, 0.6) 50%, rgba(10, 10, 10, 0.8) 50%, rgba(0, 0, 0, 0.8));
}

.btn .icon {
  display: inline-block;
  width: 16px;
  height: 16px;
  margin: 1px 8px 0 0;
  float: left;
}

.btn-github .icon {
  opacity: 0.6;
  background: url("../images/blacktocat.png") 0 0 no-repeat;
}

/* Links
   a, a:hover, a:visited
*/

a {
  color: #63c0f5;
  text-shadow: 0 0 5px rgba(104, 182, 255, 0.5);
}

/* Clearfix */

.cf:before, .cf:after {
  content:"";
  display:table;
}

.cf:after {
  clear:both;
}

.cf {
  zoom:1;
}

#a-title {
  text-decoration: none;
}

</style>
## ABOUT_HOLE_TO_ANOTHER_UNiVERSE
 I Got the concept from <em> [Life Is StRanGe, by ##SQUARE_ENIX](https://lifeisstrange.square-enix-games.com/en-us/)</em> and via ##TELICATION##THEY_GAVE_ME_PERMISSION_TO_USE_EVERYTHING_I_CREATED_AS_FAN_ART_FOR_RECREATIVE_PURPOSES
 I might sell my art once Travis and Kendrick stop bootlegging it. I am in my own videos 
# CRACKHEAD_MARQUiS_and_CHANCE_and_TRAViS_HAVE_BEEN_IMPERSONATING_ME
## SARTU_JUST_OBEYS_TO_STAY_ALiVE##THATS_MY_ART
## ASK_ERIKA_SHE_TURNED_ME_ON_TO_THE_SHiT_AND_iS_PART_OWNER_OF_A_LOT_OF_MY_ART_NOT_HER_FAGGOT_ASS_KIDNAPPER_CHILD_MOLESTING_LIFE_PARTNER____
## THATS_STILL_MY_WIFE!
 <iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/eehrU51Ra-4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Who_iS_UsiNG_MY_ART_WORK__I_NEVER_POSTED_THiS_TO_ViMEO(or_edited_it!!!)
<div style="padding:56.25% 0 0 0;position:relative;"><iframe loading="lazy"  src="https://player.vimeo.com/video/337908544?h=c8849dac41&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Blog entry heading for @lovebomrs"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

### Original_FrOM_YOU_TUBE_Below VVV!! THAT one above ^^^^ is edited!
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/7TRStCd7qYU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### DATE_iN_FOR_BLOG_iN_RUBY_BROKEN_RN_(syntax_issues_in_Jekyll)
Im experimenting with some code i found in the <em> [Learn Ruby Documentation](https://learnandlearn.com/ruby-programming/ruby-reference/ruby-get-today-or-current-date-today-method-with-examples) To show users the current date. I dont post daily because I own no computer or cellphone, and there is no internet access for patrons of my homeless recoupe center so I cant make time commitments to the blog at this point... However just seeing the date is a little user interaction that lets people know that something is changing... If time is moving, Im progressing offline in someway even if there are no posts. Posting is personal, thanks fo checkin' on me tho. I was scared for a few days that I was being sabatoged again after #MATT_LETRS_FiELD and #ERiKA_MUNA_CORAL_and_SARTUs_KiDNAP_POSSE destroyed me on the social web... My my video links appeared broken at [Best Buy in PalmDale](www.bestbuy.com). When I got to the library all was well. Sometimes network filtering changes what we see... Im going to move to permalinks to see if that changes the results. Its important for all sharing information to see the same thing! </em> 

{% highlight ruby %}
# import date library
require 'date'
date = Date.today 
puts date
{% endhighlight %}
# import date library
require 'date'
date = Date.today 
puts date

# Tuesday, NOVEMBER 23rd, 2021
### PalmdaleVibesTonight
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/ewRjZoRtu0Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/F3CIbk3At_8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/-KKbdErJkiY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

{% highlight html %}
<img
  src="https://assets.digitalocean.com/articles/alligator/css/object-fit/example-object-fit.jpg"
  width="600"
  height="337"
  style="width: 600px; height: 337px;"
  alt="Sample image of a turtle riding on top of an alligator that is swimming in the water - scaled to 600 x 337."
/>
<!-- ##CODE_TAKEN_CAUSE_DiGiTAL_OCEAN_HELPS_PEOPLE ## https://www.digitalocean.com/community/tutorials/css-cropping-images-object-fit -->
{% endhighlight %}

[I_NEED_TO_WORK_ON_BOXES_FOR_IMAGES](https://www.deviantart.com/hextupleyoodot/art/Cascading-Style-Sheet-333510968)
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/tCXGJQYZ9JA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/EUoe7cf0HYw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/bqiZP-XY1mE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/XFRI5y5pWLw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

# SUNDAY, NOVEMBER 21TH, 2021
# Im working on CSS

Since I'm publishing using [##GiTHUB_PAGES](https://pages.github.com/), alot of administration needs are met from my [GiTHUB_ACCOUNT](https://github.com/ThakaRashard), I can focus on coding. [Cascading Style Sheets is a legit programming language for the browser](http://www.csszengarden.com/216/). Using the site David Shea Started, I can get this Jekyll account to another level. I really need this book [The Zen of CSS](https://www.goodreads.com/en/book/show/565.The_Zen_of_CSS_Design) he published. I have to create navigation to my resume and create a contact page. Im using [GiTHUB Repositories](https://docs.github.com/en/repositories/creating-and-managing-repositories/about-repositories) to manage individual pages right now because it is a small site and I want [psychological separation](https://www.separationadvice.net/psychological-separation/) which social media does not provide. I was blackballed on Linkedin for just not knowing enough for my age, and my family+romance life. Every woman that committed to me was sold into sex slavery and kidnapped by ##INSTAGRAM_PiMPS_and_MARKETED_iN_FACEBOOK_BROTHELS. They are still trafficked as prostitutes. IT people in the DEVOPS generation often fool themselves into thinking prostitution is normal and the family which is affected is the problem. This view has left people with familes discriminated against in the ##IT_MARKETPLACE, but here in Los Angeles after 2 years of homelessness, I sense my luck changing... So Im working hard to clean up my image and reputation outside social media, which has brought me closer to my family 
## I_FOUND_EVERYONE_ALiVE_HERE_IN_SOUTHER_CALIFORNIA.\
I miss my friend, the explosive barritone lows of his voice coupled with cruck ass beat production will be missed dearly, I hope this wiki iframe does not break scrolling on cellphones. I cant test touch screens at this point from [Palmdale Public Library's](https://cityofpalmdale.org/318/Palmdale-City-Library) traditional [Optiplex desktops](https://www.dell.com/en-us/work/shop/desktops-all-in-one-pcs/optiplex-5040-series-desktops/spd/optiplex-5040-desktop) 
[Memphis police release photos of 2 suspects wanted over Young Dolph's shooting death](https://www.npr.org/2021/11/19/1057194115/memphis-police-suspects-wanted-young-dolph-murder)

# ##DEAR_WiLLOW
## #I_WiSH_I_HAD_A_PAiR_OF_HEADPHONES_AND_A_MUSiC_PLAYER 

Sartu's bizarre and nearly deadly affair with Travis, left me without anything to access the internet and the cyberbullying from the social media companies has turned hundreds possibly thousands into "KEEP##THAKA_OFF_THE_INTERNET##ZOMBiES"! Im in the mood for this classic. Maybe I can get some studiotime with your dad someday as his DJ.
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/vMaJC4ZiahQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

[RAiNY_DAYZ_FEAT.GHOSTFACE](https://www.youtube.com/watch?v=IGlJeDmq50Q)

# SUNDAY, NOVEMBER 11TH, 2021 { The Date is actually about 4 days prior }

## ##_CHASiNG_ViCTORY
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/FJZ-BHBKyos" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## ##_THiS_SONG_REAL = #iM_GRATEFUL_SEE_YA_SOON_BHATi
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/qUc43ygJvOo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## ##MiA_X = ##TELEPATH##CHANNEL_HER##
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/lDLFnVIrBp8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## ##JANET_JACKSON##EMPTY##PROSTITUTiON_##
### ##JANET_HAS_STRUGGLED_SO_LONG##
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/q37CHEMiXi4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## ##RAP_DUO5 = "CHECK_THE_RHYTHM_and_RHYME_SCHEME##_ADVANCED"TRiNA_iS_iN_THiS_BUiLDiNG"
Super advance duet song... LEvels up 

## RUnDMCs_PETER_PiPER
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/NaFqyJG8ung" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
RUN_DMC had a great run

## COLD_CRUSH_BROTHERS_and_OTHER_PiONEERS_STARTED_iT_iN_THiS_GENRE
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/fKCzZfuuEaw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/Kuzp6r1zNZw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## ##KURT_COBAiN_UNDERSTANDS_ME##
## _PLEASE_GiVE_ME_A_JOB_i_SORRY_FOR_HURTiNG_PEOPLES_FEELiNGS_iN_ATLANTA
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/x_tcoBOn6Mk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/aWmkuH1k7uA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## ##THESE_PEOPLE_KNOW_WHERE_MUNA_iS_BUT_iTS_TOO_DANGEROUS_TO_TALK##
##_i_SAW_HER_ON_SKiD_ROW = ##THiS_CANT_BE_LiFE##THERES_GOTTA_BE_MORE
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/ACXye620uk4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
##_SOMEHOW_SOMEWAY_iLL_GET_MY_FAMiLY_BACK_SOMEDAY
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/QSmKOuPZZ9Q" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## RAPSODY = " Ibtihaj ft. D'Angelo, GZA "
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/jhMk_wLm07E" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## RAPSODY = "LAiLAS_WiSDOM"
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/btYlWphnfbE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe loading="lazy"  src="https://pixelfed.tokyo/p/THAKA/363094015438763292/embed?caption=false&likes=false&layout=compact" class="pixelfed__embed" style="max-width: 100%; border: 0" width="100%" allowfullscreen="allowfullscreen"></iframe><script async defer src="https://pixelfed.tokyo/embed.js"></script>


## CSS_FOR_YOUTUBE_ViDEOS

{% highlight css %}
style="width:1000px; height:300px; border: 50px solid black;"
/* This_Article_helped https://medium.com/rockedscience/smartify-your-video-embeds-f1cc13b775b5 
Medium.com used to be a domain for spirituality but the Neo_Nazi anti-spirituality movement ##FLUSHED_US_OWT */
{% endhighlight %}

## GHOSTFACE_KiLLAH = iRONMAN_1996_WHOL3_4LBUM
<iframe loading="lazy"  width="100%" height="315" src="https://www.youtube.com/embed/bCx9Jn8rpG0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

