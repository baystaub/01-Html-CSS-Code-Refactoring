# 01 HTML, CSS, and Git: Code Refactor

Examples of The code prior to the Refactoring:
   " <div class="header">
        <h1>Hori<span class="seo">seo</span>n</h1>
        <div>
            <ul>
                <li>
                    <a href="#search-engine-optimization">Search Engine Optimization</a>
                </li>
                <li>
                    <a href="#online-reputation-management">Online Reputation Management</a>
                </li>
                <li>
                    <a href="#social-media-marketing">Social Media Marketing</a>
                </li>
            </ul>
        </div>
    </div>
    <div class="hero"></div>
    <div class="content">
        <div class="search-engine-optimization">
            <img src="./assets/images/search-engine-optimization.jpg" class="float-left" />
            <h2>Search Engine Optimization</h2>
            <p>
                The dominance of mobile internet use means that users are searching for the right business as they travel, shop, or sit on their couch at home. Search Engine Optimization (SEO) allows you to increase your visibility and find the right customers for your business.
            </p>
        </div>
        <div id="online-reputation-management" class="online-reputation-management">
            <img src="./assets/images/online-reputation-management.jpg" class="float-right" />
            <h2>Online Reputation Management</h2>
            <p>
                The web is full of opinions, and some of these can be negative. Social media allows anyone with an internet connection to say whatever they want about your business. Online Reputation Management gives you the control over what potential customers see when they search for your business.
            </p>
        </div>
        <div id="social-media-marketing" class="social-media-marketing">
            <img src="./assets/images/social-media-marketing.jpg" class="float-left" />
            <h2>Social Media Marketing</h2>
            <p>
                Social media continues to have a sizable influence on buying habits. Social media marketing helps you determine which platforms are suited to your brand, using analytics to find the right markets and increase your lead generation.
            </p>
        </div>
    </div>"
    
   The code works, but the problem that lies was it only used <div> tags to sepeerate the sections.
 
 So we went in and changed the core tags to:
 
 "<header class="header">
    <h1>Hori<span class="seo">seo</span>n</h1>
    <section>
      <ul>
        <li>
          <a href="#search-engine-optimization">Search Engine Optimization</a>
        </li>
        <li>
          <a href="#online-reputation-management">Online Reputation Management</a>
        </li>
        <li>
          <a href="#social-media-marketing">Social Media Marketing</a>
        </li>
      </ul>
    </section>
  </header>
  <div class="hero"></div>
  <main class="content">
    <section class="search-engine-optimization">
      <img src="./assets/images/search-engine-optimization.jpg" class="float-left" />
      <h2>Search Engine Optimization</h2>
      <p>
        The dominance of mobile internet use means that users are searching for the right business as they
        travel, shop, or sit on their couch at home. Search Engine Optimization (SEO) allows you to increase
        your visibility and find the right customers for your business.
      </p>
    </section>
    <section id="online-reputation-management" class="online-reputation-management">
      <img src="./assets/images/online-reputation-management.jpg" class="float-right" />
      <h2>Online Reputation Management</h2>
      <p>
        The web is full of opinions, and some of these can be negative. Social media allows anyone with an
        internet connection to say whatever they want about your business. Online Reputation Management gives
        you the control over what potential customers see when they search for your business.
      </p>
    </section>"
 
 We changed the main tag to a header tag, and the main content as a main tag moving into section tags in the main content.
 this did bring some problems when moving over to the css, so we ended up changing some of the code to represent the changes in the main html.
 
 example:
 
' .header section ul li {
    display: inline-block;
    margin-left: 25px;
}'

with all the changes that we made, we didnt change any of the core features and structure of the website at hand but we did make it easy to navigate the html and we cleaned up the css.

© 2021 Trilogy Education Services, LLC, a 2U, Inc. brand. Confidential and Proprietary. All Rights Reserved.
