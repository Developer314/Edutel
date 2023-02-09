---
id: home
blueprint: pages
title: Home
template: home
author: dc11e792-8eb4-4c01-aaa0-a81f48cc974e
block_types:
  -
    hero_image: banner-right-image.png
    welcome_text: 'Welcome to Edutel'
    heading: 'Best Place To Learn Graphic <em>Design!'
    button_text: 'Join Us Now!'
    tenmplate: |-
      <!-- ***** Main Banner Area Start ***** -->
        <section class="main-banner" id="top">
          <div class="container">
            <div class="row">
              <div class="col-lg-6 align-self-center">
                <div class="header-text">
                  <h6>{{welcome_text}}</h6>
                  <h2>{{heading}}</em></h2>
                  <div class="main-button-gradient">
                    <div class="scroll-to-section"><a href="{{button_link}}">{{button_text}}</a></div>
                  </div>
                </div>
              </div>
              <div class="col-lg-6">
                <div class="right-image">
                  <img src="{{hero_image}}" alt="{{heading}}">
                </div>
              </div>
            </div>
          </div>
        </section>
        <!-- ***** Main Banner Area End ***** -->
    type: home_hero
    enabled: true
    template: |-
      <!-- ***** Main Banner Area Start ***** -->
        <section class="main-banner" id="top">
          <div class="container">
            <div class="row">
              <div class="col-lg-6 align-self-center">
                <div class="header-text">
                  <h6>{{welcome_text}}</h6>
                  <h2>{{heading}}</em></h2>
                  <div class="main-button-gradient">
                    <div class="scroll-to-section"><a href="{{button_link}}">{{button_text}}</a></div>
                  </div>
                </div>
              </div>
              <div class="col-lg-6">
                <div class="right-image">
                  <img src="{{hero_image}}" alt="{{heading}}">
                </div>
              </div>
            </div>
          </div>
        </section>
        <!-- ***** Main Banner Area End ***** -->
  -
    heading_1: 'Our Services'
    heading_2: 'Provided <em>Services</em>'
    template: |-
      <section class="services" id="services">
          <div class="container">
            <div class="row">
              <div class="col-lg-12">
                <div class="section-heading">
                  <h6>{{heading_1}}</h6>
                  <h4>{{heading_2}}</h4>
                </div>
              </div>
              <div class="col-lg-12">
                <div class="owl-service-item owl-carousel">
      	          
      	        {{collection:our_services}}  
      	          
                  <div class="item">
                    <div class="service-item">
                      <div class="icon">
                        <img src="{{service_image}}" alt="{{title}}">
                      </div>
                      <h4>{{title}}</h4>
                      {{content}}
                    </div>
                  </div>
                  {{/collection:our_services}}
                  
                 
                </div>
              </div>
            </div>
          </div>
        </section>
    type: our_service
    enabled: true
  -
    block_title: 'OUR COURSES'
    sub_title: 'What You Can <em>Learn</em>'
    some_data: 'You just think about TemplateMo whenever you need free CSS templates for your business website'
    template: |-
      <section class="our-courses" id="courses">
          <div class="container">
            <div class="row">
              <div class="col-lg-6 offset-lg-3">
                <div class="section-heading">
                  <h6>{{block_title}}</h6>
                  <h4>{{sub_title}}</h4>
                  <p>{{some_data}}</p>
                </div>
              </div>
              <div class="col-lg-12">
                <div class="naccs">
                  <div class="tabs">
                    <div class="row">
                      <div class="col-lg-3">
                        <div class="menu">
      	                
                      
      	                {{collection:our_courses}}  
      	                  
                          <div class="{{ if first }} active {{/if}} gradient-border"><span>{{title}}</span></div>
                          {{/collection:our_courses}} 
                        </div>
                      </div>
                      <div class="col-lg-9">
      	               
                        <ul class="nacc">
      	                  
      	                  
      	                {{collection:our_courses}}    
      	                  
                          <li class="{{ if first }} active {{/if}}">
                            <div>
                              <div class="left-image">
                                <img src="{{course_image}}" alt="{{title}}">
                                <div class="price"><h6>{{price}}</h6></div>
                              </div>
                              <div class="right-content">
                                <h4>{{title}}</h4>
                                {{content}}
                                <span>{{hours}}</span>
                                <span>{{weeks}}</span>
                                <span class="last-span">{{certificates}}</span>
                                <div class="text-button">
                                  <a href="{{course_link}}" target="{{link_target}}">{{label}}</a>
                                </div>
                              </div>
                            </div>
                          </li>
                       {{/collection:our_courses}} 
                          </ul>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </section>
    type: our_courses
    enabled: true
  -
    image: cta-left-image.png
    title_1: 'Get the sale right now!'
    title_2: 'Up to 50% OFF For 1+ courses'
    description: "Kogi VHS freegan bicycle rights try-hard green juice probably haven't heard of them cliche la croix af chillwave."
    button_text: 'View Courses'
    button_link: 'http://www.google.com'
    link_target: _blank
    template: |-
      <section class="simple-cta">
          <div class="container">
            <div class="row">
              <div class="col-lg-5 offset-lg-1">
                <div class="left-image">
                  <img src="{{image}}" alt="{{title_1}}">
                </div>
              </div>
              <div class="col-lg-5 align-self-center">
                <h6>{{title_1}}</h6>
                <h4>{{title_2}}</h4>
                <p>{{description}}</p>
                <div class="white-button">
                  <a href="{{button_link}}" target="{{link_target}}">{{button_text}}</a>
                </div>
              </div>
            </div>
          </div>
        </section>
    type: highlight_box
    enabled: true
  -
    title_1: Testimonials
    title_2: 'What They <em>Think</em>'
    template: |-
      <section class="testimonials" id="testimonials">
          <div class="container">
            <div class="row">
              <div class="col-lg-12">
                <div class="section-heading">
                  <h6>{{title_1}}</h6>
                  <h4>{{title_2}}</h4>
                </div>
              </div>
              <div class="col-lg-12">
                <div class="owl-testimonials owl-carousel" style="position: relative; z-index: 5;">
      	          
      	          {{collection:testimonials}}  
                  <div class="item">
                    {{content}}
                      <h4>{{title}}</h4>
                      <span>{{designation}}</span>
                      <img src="{{icon}}" alt="{{title}}">
                  </div>
                  
                  {{/collection:testimonials}}  
            
                </div>
              </div>
            </div>
          </div>
        </section>
    type: testimonials
    enabled: true
    icon: quote.png
updated_by: dc11e792-8eb4-4c01-aaa0-a81f48cc974e
updated_at: 1675839895
published: true
---
## Welcome to your new brand Statamic site!

Not sure where to do next? Here are a few ideas, but feel free to explore in your own way, in your own time.

- [Jump into the Control Panel](/cp) and edit this page or begin setting up your own collections and blueprints.
- [Head to the docs](https://statamic.dev) and learn how Statamic works.
- [Watch some Statamic videos](https://youtube.com/statamic) on YouTube.
- [Join our Discord chat](https://statamic.com/discord) and meet thousands of other Statamic developers.
- [Start a discussion](https://github.com/statamic/cms/discussions) and get answers to your questions.
- [Star Statamic on Github](https://github.com/statamic/cms) if you enjoy using it!