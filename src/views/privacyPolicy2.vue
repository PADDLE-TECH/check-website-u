<template>
  <div class="policy">
    <div class="color"></div>
    <appHeader></appHeader>
    <div class="container-fluid">
        <div class="row superHeader">
            <h1 >Privacy Policy</h1>
        </div>

        <div class="row">
            <div class="col-md-4">
                <div class="box">
                    <h2>Table of Content  </h2>
                    <a href="#1"><h3 class="first-content" :class="read1 ? 'active' : 'notActive'" @click="read1 = !read1">We are here to protect you?</h3></a>
                    <hr>
                    <a href="#2"><h3 :class="read2 ? 'active' : 'notActive'" @click="read2 = !read2">Definitions and key terms</h3></a>
                    <hr>
                    <a href="#3"><h3 :class="read3 ? 'active' : 'notActive'" @click="read3 = !read3">What Information Do We Collect?</h3></a>
                    <hr>
                    <a href="#4"><h3 :class="read4 ? 'active' : 'notActive'" @click="read4 = !read4">How Do We Use The Information we collect?</h3></a>
                    <hr>
                    <a href="#5"><h3 :class="read5 ? 'active' : 'notActive'" @click="read5 = !read5">When does check retail use end user information from third parties?</h3></a>
                    <hr>

                    <a href="#6"><h3 :class="read6 ? 'active' : 'notActive'" @click="read6 = !read6">When does check retail use customer information from third parties?</h3></a>
                    <hr>
                    <a href="#7"><h3 :class="read7 ? 'active' : 'notActive'" @click="read7 = !read7">Do we share the information we collect with third parties?</h3></a>
                    <hr>
                    <a href="#8"><h3 :class="read8 ? 'active' : 'notActive'" @click="read8 = !read8">Where and when is information collected from customers and end users?</h3></a>
                    <hr>
                    <a href="#9"><h3 :class="read9 ? 'active' : 'notActive'" @click="read9 = !read9">How Do We Protect Your Information?</h3></a>
                    <hr>
                    <a href="#10"><h3 :class="read10 ? 'active' : 'notActive'" @click="read10 = !read10">Could my information be transferred to other countries?</h3></a>
                    <hr>
                    <a href="#11"><h3 :class="read11 ? 'active' : 'notActive'" @click="read11= !read11">Is the information collected through the check retail Service secure?</h3></a>
                    <hr>
                    <a href="#12"><h3 :class="read12 ? 'active' : 'notActive'" @click="read12 = !read12">Personnel</h3></a>
                    <hr>
                    <a href="#13"><h3 :class="read13 ? 'active' : 'notActive'" @click="read13 = !read13">Affiliates</h3></a>
                    <hr>
                    <a href="#14"><h3 :class="read14 ? 'active' : 'notActive'" @click="read14 = !read14">Governing Law</h3></a>
                    <hr>
                    <a href="#15"><h3 :class="read15 ? 'active' : 'notActive'" @click="read15 = !read15">Your Consent</h3></a>
                    <hr>

                    <a href="#16"><h3 :class="read16 ? 'active' : 'notActive'" @click="read16 = !read16">Payment Detail</h3></a>
                    <hr>
                    <a href="#17"><h3 :class="read17 ? 'active' : 'notActive'" @click="read17 = !read17">Kids' Privacy</h3></a>
                    <hr>
                    <a href="#18"><h3 :class="read18 ? 'active' : 'notActive'" @click="read18 = !read18">Changes To Our Privacy Policy</h3></a>
                    <hr>
                    <a href="#19"><h3 :class="read19 ? 'active' : 'notActive'" @click="read19 = !read19">Third-Party Services</h3></a>
                    <hr>
                    <a href="#20"><h3 :class="read20 ? 'active' : 'notActive'" @click="read20 = !read20">Tracking Technologies</h3></a>
                    <hr>
                    <a href="#21"><h3 :class="read21 ? 'active' : 'notActive'" @click="read21 = !read21">What is personal data</h3></a>
                    <hr>
                    <a href="#22"><h3 :class="read22 ? 'active' : 'notActive'" @click="read22 = !read22">The Data Protection Principles include requirements such as:</h3></a>
                    <hr>
                    <a href="#23"><h3 :class="read23 ? 'active' : 'notActive'" @click="read23 = !read23">Contact Us</h3></a>
                    <!--<hr>-->
                </div>
            </div>
            <div class="col-md-8 section-box">
                <section id="1" class="section1" :class="read1 ? 'active-section' : 'notActive'">
                    <h2 @click="read1 = !read1" :class="read1 ? 'active' : 'notActive'">We are here to protect you?<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read1 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read1 = !read1"  :class="read1 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read1">Check retail is committed to protecting your privacy. This Privacy Policy explains how your personal informationis collected, used, and disclosed by check retail.<br><br>This Privacy Policy applies to our website, and its associated subdomains (collectively, our “Service”) alongside our application, check retail. By accessing or using our Service, you signify that you have read, understood, and agree to our collection, storage, use, and disclosure of your personal information as described in this Privacy Policy and our Terms of Service</p>
                </section>

                <section id="2" :class="read2 ? 'active-section' : 'notActive'">
                    <h2 @click="read2 = !read2" :class="read2 ? 'active' : 'notActive'">Definitions and key terms<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read2 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read2 = !read2"  :class="read2 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read2">
                        <span><p>
                            To help explain things as clearly as possible in this Privacy Policy, every time any of these
                            terms are referenced, are strictly defined as:<br><br>

                    <!--<ul>
                        <li><img src="../assets/images2/orange-dot.png">Cookie: small amount of data generated by a website and saved by your web browser. It is used to identify your browser, provide analytics, remember information about you such as your language preference or login information.</li>
                    </ul>-->

                            <table>
                            <tr>
                                <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                                <td><p>Cookie: small amount of data generated by a website and saved by your web browser. It is used to identify your browser, provide analytics, remember information about you such as your language preference or login information.</p></td>
                            </tr>

                            <tr>
                                <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                                <td><p>Company: when this policy mentions “Company,” “we,” “us,” or “our,” it refers to paddle technologies, (14, ORANGE GATE, PLAMER STREET, OLUYOLE ESTATE IBADAN, IBADAN, OYO STATE, NIGERIA) that is responsible for your information under this Privacy Policy.</p></td>
                            </tr>

                            <tr v-show="showMore1">
                                <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                                <td><p>Country: where check retail or the owners/founders of check retail are based, in this case is Nigeria</p></td>
                            </tr>

                            <tr v-show="showMore1">
                                <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                                <td><p>Customer: refers to the company, organization or person that signs up to use the check retail Service to manage the relationships with your consumers or service users.</p></td>
                            </tr>

                            <tr v-show="showMore1">
                                <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                                <td><p>Device: any internet connected device such as a phone, tablet, computer or any other device that can be used to visit check retail and use the services.</p></td>
                            </tr>

                            <tr v-show="showMore1">
                                <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                                <td><p>Personnel: refers to those individuals who are employed by check retail or are under contract to perform a service on behalf of one of the parties.</p></td>
                            </tr>

                            <tr v-show="showMore1">
                                <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                                <td><p>Personal Data: any information that directly, indirectly, or in connection with other information — including a personal identification number — allows for the identification or identifiability of a natural person.</p></td>
                            </tr>

                            <tr v-show="showMore1">
                                <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                                <td><p>Service: refers to the service provided by check retail as described in the relative terms (if available) and on this platform.</p></td>
                            </tr>

                            <tr v-show="showMore1">
                                <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                                <td><p>Third-party service: refers to advertisers, contest sponsors, promotional and marketing partners, and others who provide our content or whose products or services we think may interest you.</p></td>
                            </tr>

                            <tr v-show="showMore1">
                                <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                                <td><p>Website/APP: check retail."’s" site, which can be accessed via this URL:</p></td>
                            </tr>

                            <tr v-show="showMore1">
                                <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                                <td><p>You: a person or entity that is registered with check retail to use the Services.</p></td>
                            </tr>
                            </table>
                            <button class="" v-show="!showMore1" @click="showMore1 = !showMore1">Read More</button>
                            <button class="" v-show="showMore1" @click="showMore1 = !showMore1">Show Less</button>

                            <!--<button class="close-btn btn-color2" v-show="read2" @click="read2 = !read2"><span class="close-text">Close</span> <img src="../assets/images/Vector-caret-up.png" class="caret2" ></button>-->
                        </p></span>



                    </p>
                </section>

                <section id="3" :class="read3 ? 'active-section' : 'notActive'">
                    <h2 @click="read3 = !read3" :class="read3 ? 'active' : 'notActive'">What Information Do We Collect?<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read3 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read3 = !read3"  :class="read3 ? 'rotate' : 'rotateBack'"></i>
                    <span v-show="read3">
                    <p >
                      We collect information from you when you visit our app, register on our site, place an order, subscribe to our newsletter, respond to a survey or fill out a form.</p>

                      <table class="section3-table">
                        <tr>
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>Name / Username</p></td>
                        </tr>
                        <tr>
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>Phone Numbers</p></td>
                        </tr>
                        <tr>
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>Email Addresses</p></td>
                        </tr>
                        <tr>
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>Mailing Addresses</p></td>
                        </tr>
                        <tr>
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>Password</p></td>
                        </tr>
                        <tr>
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>Gender</p></td>
                        </tr><br><br>

                      </table>
                        <p v-show="showMore2">We also collect information from mobile devices for a better user experience, although these features are completely optional:</p>


                      <table>
                        <tr v-show="showMore2">
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>Photo Gallery (Pictures): Granting photo gallery access allows the user to upload any picture from their photo gallery, you can safely deny photo gallery access for this app.</p></td>
                        </tr>
                      </table>
                      <p>
                      <button class="read-more-btn" v-show="!showMore2" @click="showMore2 = !showMore2">Read More</button>
                      <button class="read-more-btn" v-show="showMore2" @click="showMore2 = !showMore2">Show Less</button>

                      <!--<button class="close-btn btn-color3" v-show="read3" @click="read3 = !read3"><span class="close-text">Close</span> <img src="../assets/images/Vector-caret-up.png" class="caret2" ></button>-->
                      </p>
                      </span>
                </section>

                <section id="4" :class="read4 ? 'active-section' : 'notActive'">
                    <h2 @click="read4 = !read4" :class="read4 ? 'active' : 'notActive'">How Do We Use The Information we collect?<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read4 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read4 = !read4"  :class="read4 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read4"><span>Any of the information we collect from you may be used in one of the following ways:<br>
                      <table>
                        <tr>
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>To personalize your experience (your information helps us to better respond to your individual needs)</p></td>
                        </tr>

                        <tr>
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>To improve our app (we continually strive to improve our app offerings based on the information and feedback we receive from you)</p></td>
                        </tr>

                        <tr v-show="showMore3">
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>To improve customer service (your information helps us to more effectively respond to your customer service requests and support needs)</p></td>
                        </tr>

                        <tr v-show="showMore3">
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>To process transactions</p></td>
                        </tr>

                        <tr v-show="showMore3">
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>Enabling you to participate in promotions, competitions and surveys.</p></td>
                        </tr>

                        <tr v-show="showMore3">
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>Complying with our legal obligations, including verifying your identity where necessary.</p></td>
                        </tr>

                        <tr v-show="showMore3">
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>Detecting fraud.</p>

                            <tr v-show="showMore3">
                              <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                              <td><p>To administer a contest, promotion, survey or other site feature</p></td>
                            </tr>
                            <tr v-show="showMore3">
                              <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                              <td><p>To send periodic emails</p></td>
                            </tr>
                          </td>
                        </tr>
                      </table>
                      <button class="read-more-btn" v-show="!showMore3" @click="showMore3 = !showMore3">Read More</button>
                      <button class="read-more-btn" v-show="showMore3" @click="showMore3 = !showMore3">Show Less</button>

                      <!--<button class="close-btn btn-color4" v-show="read4" @click="read4 = !read4"><span class="close-text">Close</span> <img src="../assets/images/Vector-caret-up.png" class="caret2" ></button><br><br>-->
                    </span></p>
                </section>


                <!--Testing Part-->
                <section id="5" :class="read5 ? 'active-section' : 'notActive'">
                    <h2 @click="read5 = !read5" :class="read5 ? 'active' : 'notActive'">When does check retail use end user information from third parties?<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read5 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read5 = !read5"  :class="read5 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read5"><span>
                      Check retail will collect End User Data necessary to provide the check retail services to our customers.<br><br>

                      End users may voluntarily provide us with information they have made available on social media websites. If you provide us with any such information, we may collect publicly available information from the social media websites you have indicated. You can control how much of your information social media websites make public by visiting these websites and changing your privacy settings.<br>
                      <!--<button class="close-btn btn-color1" v-show="read5" @click="read5 = !read5"><span class="close-text">Close</span> <img src="../assets/images/Vector-caret-up.png" class="caret2" ></button>-->
                      </span></p>
                </section>

                <section id="6" :class="read6 ? 'active-section' : 'notActive'">
                    <h2 @click="read6 = !read6" :class="read6 ? 'active' : 'notActive'">When does check retail use customer information from third parties?<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read6 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read6 = !read6"  :class="read6 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read6">
                        <span>We receive some information from the third parties when you contact us. For example, when you submit your email address to us to show interest in becoming a check retail customer, we receive information from a third party that provides automated fraud detection services to check retail. We also occasionally collect information that is made publicly available on social media websites. You can control how much of your information social media websites make public by visiting these websites and changing your privacy settings.</span>
                    </p>
                </section>

                <section id="7" :class="read7 ? 'active-section' : 'notActive'">
                    <h2 @click="read7 = !read7" :class="read7 ? 'active' : 'notActive'">Do we share the information we collect with third parties?<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read7 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read7 = !read7"  :class="read7 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read7">
                        <span>
                            We may share the information that we collect, both personal and non-personal, with third parties such as advertisers, contest sponsors, promotional and marketing partners, and others who provide our content or whose products or services we think may interest you. We may also share it with our current and future affiliated companies and business partners, and if we are involved in a merger, asset sale or other business reorganization, we may also share or transfer your personal and non-personal information to our successors-in-interest.<br><br>
                        </span>

                    <span v-show="showMore4">
                      We may engage trusted third party service providers to perform functions and provide services to us, such as hosting and maintaining our servers and the app, database storage and management, e-mail management, storage marketing, credit card processing, customer service and fulfilling orders for products and services you may purchase through the app. We will likely share your personal information, and possibly some non-personal information, with these third parties to enable them to perform these services for us and for you.<br><br>

                      We may share portions of our log file data, including IP addresses, for analytics purposes with third parties such as web analytics partners, application developers, and ad networks. If your IP address is shared, it may be used to estimate general location and other technographics such as connection speed, whether you have visited the app in a shared location, and type of the device used to visit the app. They may aggregate information about our advertising and what you see on the app and then provide auditing, research and reporting for us and our advertisers.<br><br>

                      We may also disclose personal and non-personal information about you to government or law enforcement officials or private parties as we, in our sole discretion, believe necessary or appropriate in order to respond to claims, legal process (including subpoenas), to protect our rights and interests or those of a third party, the safety of the public or any person, to prevent or stop any illegal, unethical, or legally actionable activity, or to otherwise comply with applicable court orders, laws, rules and regulations.<br><br>
                    </span>

                    <button class="read-more-btn" v-show="!showMore4" @click="showMore4 = !showMore4">Read More</button>
                    <button class="read-more-btn" v-show="showMore4" @click="showMore4 = !showMore4">Show Less</button><br>
                    <!--<button class="close-btn btn-color3" v-show="read7" @click="read7 = !read7"><span class="close-text">Close</span> <img src="../assets/images/Vector-caret-up.png" class="caret2" ></button>-->

                    </p>
                </section>

                <section id="8" :class="read8 ? 'active-section' : 'notActive'">
                    <h2 @click="read8 = !read8" :class="read8 ? 'active' : 'notActive'">Where and when is information collected from customers and end users?<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read8 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read8 = !read8"  :class="read8 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read8">Check retail will collect personal information that you submit to us. We may also receive personal information about you from third parties as described above</p>
                </section>

                <section id="9" :class="read9 ? 'active-section' : 'notActive'">
                    <h2 @click="read9 = !read9" :class="read9 ? 'active' : 'notActive'">How Do We Protect Your Information?<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read9 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read9 = !read9"  :class="read9 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read9"> We implement a variety of security measures to maintain the safety of your personal information when you place an order or enter, submit, or access your personal information. We offer the use of a secure server. All supplied sensitive/credit information is transmitted via Secure Socket Layer (SSL) technology and then encrypted into our Payment gateway providers database only to be accessible by those authorized with special access rights to such systems, and are required to keep the information confidential. After a transaction, your private information (credit cards, social security numbers, financials, etc.) is never kept on file. We cannot, however, ensure or warrant the absolute security of any information you transmit to check retail or guarantee that your information on the Service may not be accessed, disclosed, altered, or destroyed by a breach of any of our physical, technical, or managerial safeguards.</p>
                </section>



                <section id="10" :class="read10 ? 'active-section' : 'notActive'">
                    <h2 @click="read10 = !read10" :class="read10 ? 'active' : 'notActive'">Could my information be transferred to other countries?<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read10 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read10 = !read10"  :class="read10 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read10">Check retail is incorporated in Nigeria. Information collected via our website, through direct interactions with you, or from use of our help services may be transferred from time to time to our offices or personnel, or to third parties, located throughout the world, and may be viewed and hosted anywhere in the world, including countries that may not have laws of general applicability regulating the use and transfer of such data. To the fullest extent allowed by applicable law, by using any of the above, you voluntarily consent to the trans-border transfer and hosting of such information.</p>
                </section>

                <section id="11" :class="read11 ? 'active-section' : 'notActive'">
                    <h2 @click="read11 = !read11" :class="read11 ? 'active' : 'notActive'">Is the information collected through the check retail Service secure?<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read11 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read11 = !read11"  :class="read11 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read11">We take precautions to protect the security of your information. We have physical, electronic, and managerial procedures to help safeguard, prevent unauthorized access, maintain data security, and correctly use your information. However, neither people nor security systems are foolproof, including encryption systems. In addition, people can commit intentional crimes, make mistakes or fail to follow policies. Therefore, while we use reasonable efforts to protect your personal information, we cannot guarantee its absolute security. If applicable law imposes any non-disclaimable duty to protect your personal information, you agree that intentional misconduct will be the standards used to measure our compliance with that duty.</p>
                </section>

                <section id="12" :class="read12 ? 'active-section' : 'notActive'">
                    <h2 @click="read12 = !read12" :class="read12 ? 'active' : 'notActive'">Personnel<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read12 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read12 = !read12"  :class="read12 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read12">f you are a check retail worker or applicant, we collect information you voluntarily provide to us. We use the information collected for Human Resources purposes in order to administer benefits to workers and screen applicants.<br><br>

                      You may contact us in order to <br>(1) update or correct your information, <br>(2) change your preferences with respect to communications and other information you receive from us, or <br>(3) receive a record of the information we have relating to you. Such updates, corrections, changes and deletions will have no effect on other information that we maintain, or information that we have provided to third parties in accordance with this Privacy Policy prior to such update, correction, change or deletion.</p>
                </section>

                <section id="13" :class="read13 ? 'active-section' : 'notActive'">
                    <h2 @click="read13 = !read13" :class="read13 ? 'active' : 'notActive'">Affiliates<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read13 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read13 = !read13"  :class="read13 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read13">We may disclose information (including personal information) about you to our Corporate Affiliates. For purposes of this Privacy Policy, "Corporate Affiliate" means any person or entity which directly or indirectly controls, is controlled by or is under common control with check retail, whether by ownership or otherwise. Any information relating to you that we provide to our Corporate Affiliates will be treated by those Corporate Affiliates in accordance with the terms of this Privacy Policy.</p>
                </section>

                <section id="14" :class="read14 ? 'active-section' : 'notActive'">
                    <h2 @click="read14 = !read14" :class="read14 ? 'active' : 'notActive'">Governing Law<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read14 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read14 = !read14"  :class="read14 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read14">This Privacy Policy is governed by the laws of Nigeria without regard to its conflict of laws provision. You consent to the exclusive jurisdiction of the courts in connection with any action or dispute arising between the parties under or in connection with this Privacy Policy except for those individuals who may have rights to make claims under Privacy Shield, or the Swiss-US framework.<br><br>

                      The laws of Nigeria, excluding its conflicts of law rules, shall govern this Agreement and your use of the app. Your use of the app may also be subject to other local, state, national, or international laws.<br><br>

                      By using check retail or contacting us directly, you signify your acceptance of this Privacy Policy. If you do not agree to this Privacy Policy, you should not engage with our website, or use our services. Continued use of the website, direct engagement with us, or following the posting of changes to this Privacy Policy that do not significantly affect the use or disclosure of your personal information will mean that you accept those changes.</p>
                </section>






                <section id="15" :class="read15 ? 'active-section' : 'notActive'">
                    <h2 @click="read15 = !read15" :class="read15 ? 'active' : 'notActive'">Your Consent<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read15 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read15 = !read15"  :class="read15 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read15">We've updated our Privacy Policy to provide you with complete transparency into what is being set when you visit our site and how it's being used. By using our app, registering an account, or making a purchase, you hereby consent to our Privacy Policy and agree to its terms.</p>
                </section>

                <section id="16" :class="read16 ? 'active-section' : 'notActive'">
                    <h2 @click="read16 = !read16" :class="read16 ? 'active' : 'notActive'">Payment Detail<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read16 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read16 = !read16"  :class="read16 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read16">In respect to any credit card or other payment processing details you have provided us, we commit that this confidential information will be stored in the most secure manner possible.</p>
                </section>

                <section id="17" :class="read17 ? 'active-section' : 'notActive'">
                    <h2 @click="read17 = !read17" :class="read17 ? 'active' : 'notActive'">Kids' Privacy<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read17 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read17 = !read17"  :class="read17 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read17">We collect information from kids under the age of 13 just to better our services. If You are a parent or guardian and You are aware that Your child has provided Us with Personal Data without your permission, please contact Us. If We become aware that We have collected Personal Data from anyone under the age of 13 without verification of parental consent, We take steps to remove that information from Our servers.</p>
                </section>

                <section id="18" :class="read18 ? 'active-section' : 'notActive'">
                    <h2 @click="read18 = !read18" :class="read18 ? 'active' : 'notActive'">Changes To Our Privacy Policy<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read18 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read18 = !read18"  :class="read18 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read18">We may change our Service and policies, and we may need to make changes to this Privacy Policy so that they accurately reflect our Service and policies. Unless otherwise required by law, we will notify you (for example, through our Service) before we make changes to this Privacy Policy and give you an opportunity to review them before they go into effect. Then, if you continue to use the Service, you will be bound by the updated Privacy Policy. If you do not want to agree to this or any updated Privacy Policy, you can delete your account.</p>
                </section>

                <section id="19" :class="read19 ? 'active-section' : 'notActive'">
                    <h2 @click="read19 = !read19" :class="read19 ? 'active' : 'notActive'">Third-Party Services<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read19 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read19 = !read19"  :class="read19 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read19">We may display, include or make available third-party content (including data, information, applications and other products services) or provide links to third-party websites or services ("Third- Party Services").
                      You acknowledge and agree that check retail shall not be responsible for any Third-Party Services, including their accuracy, completeness, timeliness, validity, copyright compliance, legality, decency, quality or any other aspect thereof. check retail does not assume and shall not have any liability or responsibility to you or any other person or entity for any Third-Party Services.<br><br>

                      Third-Party Services and links thereto are provided solely as a convenience to you and you access and use them entirely at your own risk and subject to such third parties' terms and conditions.</p>
                </section>

                <section id="20" :class="read20 ? 'active-section' : 'notActive'">
                    <h2 @click="read20 = !read20" :class="read20 ? 'active' : 'notActive'">Tracking Technologies<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read20 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read20 = !read20"  :class="read20 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read20">Google Maps API<br><br>
                      Google Maps API is a robust tool that can be used to create a custom map, a searchable map, check-in functions, display live data synching with location, plan routes, or create a mashup just to name a few.<br><br>

                      Google Maps API may collect information from You and from Your Device for security purposes.<br><br>

                      Google Maps API collects information that is held in accordance with its Privacy Policy</p>
                </section>

                <section id="21" :class="read21 ? 'active-section' : 'notActive'">
                    <h2 @click="read21 = !read21" :class="read21 ? 'active' : 'notActive'">What is personal data<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read21 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read21 = !read21"  :class="read21 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read21">Any data that relates to an identifiable or identified individual. GDPR covers a broad spectrum of information that could be used on its own, or in combination with other pieces of information, to identify a person. Personal data extends beyond a person’s name or email address. Some examples include financial information, political opinions, genetic data, biometric data, IP addresses, physical address, sexual orientation, and ethnicity</p>
                </section>

                <section id="22" :class="read22 ? 'active-section' : 'notActive'">
                    <h2 @click="read22 = !read22" :class="read22 ? 'active' : 'notActive'">The Data Protection Principles include requirements such as:<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read22 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read22 = !read22"  :class="read22 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read22">
                        <table class="section3-table">
                        <tr>
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>Personal data collected must be processed in a fair, legal, and transparent way and should only be used in a way that a person would reasonably expect.</p></td>
                        </tr>
                        <tr>
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>Personal data should only be collected to fulfil a specific purpose and it should only be used for that purpose. Organizations must specify why they need the personal data when they collect it.</p></td>
                        </tr>
                        <tr>
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>Personal data should be held no longer than necessary to fulfil its purpose</p></td>
                        </tr>
                        <tr>
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>People covered by the GDPR have the right to access their own personal data. They can also request a copy of their data, and that their data be updated, deleted, restricted, or moved to another organization.</p></td>
                        </tr>
                      </table>
                    </p>
                </section>

                <section id="23" :class="read23 ? 'active-section' : 'notActive'">
                    <h2 @click="read23 = !read23" :class="read23 ? 'active' : 'notActive'">Contact Us<i class="fa fa-angle-right arrow" aria-hidden="true"  :class="read23 ? 'rotate' : 'rotateBack'"></i></h2>
                    <i class="fa fa-angle-right arrow-mobile" aria-hidden="true" @click="read23 = !read23"  :class="read23 ? 'rotate' : 'rotateBack'"></i>
                    <p v-show="read23">
                        Don't hesitate to contact us if you have any questions.<br><br>

                      <table class="section3-table">
                        <tr>
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>Via Email:  hello.paddle@gmail.com</p></td>
                        </tr>
                        <tr>
                          <td><p><img src="../assets/images2/orange-dot.png" class="mark-icon"></p></td>
                          <td><p>Via Phone Number:  08149734622</p></td>
                        </tr>
                      </table>
                    </p>
                </section>
            </div>
        </div>

    </div>
    <footerLinks></footerLinks>

  </div>
</template>

<script>
import appHeader from '../components/headerNav.vue';
import footerLinks from '../components/linksFooter.vue';

export default {
  name: 'privacyPolicy',
  components: {
    appHeader,
    footerLinks

  },
  data () {
    return {
      showMore1: false,
      showMore2: false,
      showMore3: false,
      showMore4: false,
      read1: false,
      read2: false,
      read3: false,
      read4: false,
      read5: false,
      read6: false,
      read7: false,
      read8: false,
      read9: false,
      read10: false,
      read11: false,
      read12: false,
      read13: false,
      read14: false,
      read15: false,
      read16: false,
      read17: false,
      read18: false,
      read19: false,
      read20: false,
      read21: false,
      read22: false,
      read23: false
    }
  }
}

</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500&family=Poppins:wght@300;500;600&display=swap');
@import url('http://fonts.cdnfonts.com/css/euclid-circular-a');

/*.container {
    position: relative;
}*/

.box::-webkit-scrollbar {
  width: 12px;               /* width of the entire scrollbar */
}

.box::-webkit-scrollbar-track {
  background: rgb(230, 227, 227);        /* color of the tracking area */
}

.box::-webkit-scrollbar-thumb {
  background-color: #FF9F24;    /* color of the scroll thumb */
  border-radius: 20px;       /* roundness of the scroll thumb */

  border: 3px solid  rgb(230, 227, 227); /* creates padding around scroll thumb */
}

.superHeader h1 {
    font-family: 'Euclid Circular A';
    font-style: normal;
    font-weight: 600;
    font-size: 80px;
    line-height: 90px;
    align-items: center;
    letter-spacing: -0.05em;
    color: #000000;
    margin-top: 187px;
}
.superHeader {
    display: flex;
    align-items: center;
    justify-content: center;
}
.box a {
    text-decoration: none;
    color: #130B01;
}
.box {
    border: 1px solid #DEDEDE;
    text-align: left;
    width: 304px;
    padding: 24px 24px 32px;
    border-radius: 12px;
    margin-left: 70px;
    margin-top: 63px;
    position: sticky;
    top: 0;
    overflow-y: scroll;
    height: 700px;

    margin-bottom: 50px;
}
.box h2 {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 600;
    font-size: 24px;
    color: #130B01;
}
.box h3 {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 24px;


    display: inline-block;
    width: 200px;
    white-space: nowrap;
    overflow: hidden !important;
    text-overflow: ellipsis;
}
.box .first-content{
    margin-top: 32px;
}
.section-box {
    margin-bottom: 50px;
}
section {
    font-family: 'Poppins';
    padding: 24px;
    text-align: left;
    border: 1px solid #DEDEDE;
    border-radius: 12px;
    margin-left: -50px;
    width: 800px;
    transition: all 0.4s ease;
    position: relative;
    margin-top: 24px;
}
section h2{
    color: #130B01;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 600;
    font-size: 16px;
    line-height: 24px;
}
section h2:hover {
    cursor: pointer;
    color: #f7c075;
}
section p {
    font-weight: 400;
    font-size: 14px;
    line-height: 24px;
    color: #888580;
}
section button {
    border: 1px solid #FF9F24;
    border-radius: 5px;
    padding: 5px 10px;
    background: #fff;
    transition: all 0.4s ease;
}
section button:hover {
    transform: scale(1.02);
    background: #f7c075;
    color: #fff;
    transition: all 0.4s ease;
}
section button:active {
    transform: scale(1.02);
    background: #f7c075;
    color: #fff;
    transition: all 0.4s ease;
}
.section1 {
    margin-top: 63px;
}
.arrow {
    height: 16px;
    width: 16px;
    float: right;
    margin-right: 3px;
}

.rotate {
    transform: rotate(90deg);
    transition: all 0.4s ease;
    color: #FF9F24;
}
.rotateBack {
    transform: rotate(0deg);
    transition: all 0.4s ease;
}
.active {
    color: #FF9F24;
}
.active-section {
    border: 1px solid #FF9F24;
    transform: scale(1.03);
    transition: all 0.4s ease;
}
.arrow-mobile {
    display: none;
}
/*ul {
    margin-left: -30px;
}
li {
    list-style: none;
}*/
td img {
    width: 10px;
    height: 10px;
    margin-right: 10px;
}
table {
  margin-left: 0%;
}
/*table td {
  margin-left: 0%;
}*/
table td {
  vertical-align: top;
}
.mark-icon {
  margin-right: 5px;
}

@media screen and (max-width: 800px) {
    .policy {
        overflow-x: hidden;
        /*padding: 20px;*/
    }
    /*.container {
        padding: 20px;
    }*/
    .superHeader h1 {
        font-size: 60px;
        line-height: 60px;
        margin-top: 30px;
    }
    .box {
        margin-left: 0px;
        width: auto;
        height: 400px;
    }
    .box h3 {
        display: inline-block;
        width: 250px;
        white-space: nowrap;
        overflow: hidden !important;
        text-overflow: ellipsis;
    }
    section {
        padding: 16px;
        text-align: left;
        border-radius: 12px;
        margin-left: 0px;
        width: auto;
        /*width: 200px;*/
        transition: all 0.4s ease;
        position: relative;
        /*margin-top: 24px;*/
    }
    section h2 {
        width: 250px;
        display: inline-block;
    }
    .arrow-mobile {
        height: 16px;
        width: 16px;
        /*float: right;*/
        margin-right: 3px;
        position: absolute;
        right: 10px;
        display: inline-block;
        transform:translateY(3px);
    }
    .arrow {
        display: none;
    }
}
</style>