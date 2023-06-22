<script>
    import Modal from './Modal.svelte';

    let showModal1, showModal2, showModal3, showModal4, showModal5 = false;
</script>
<style>
     .page-content {
        width: 85%;
        margin: 0 auto;
        margin-bottom: 5rem;
        padding-top: 4rem;
    }
    .page-content p {
        font-family: "Now Alt";
        font-size: 20px;
        line-height: 50px;
        font-weight: 400;
        font-style: normal;
    }
    .page-content h2 {
        text-transform: uppercase;
    }
    .container {
        width: 627px;
        height: 3px;
        background-color: #3C9E36;
        position: relative;
        margin-bottom: 100px;
        left: 34px;
    }
    .circle {
        display: inline-block;
        vertical-align: left;
        width: 15px;
        height: 15px;
        background-color: #3C9E36;
        border: solid 1px #3C9E36;
        border-radius: 50%;
        position: absolute;
        top: -8px;
        left: -23px;
    }
    .container.inverse {
        left: -85px;
    }
    .circle.inverse {
        left: 101%;
    }
    .readmore {
        text-transform: uppercase;
        font-size: 13px;
        font-family: "Now Alt";
        font-weight: 700;
        color: #fff;
        background-color: #3C9E36;
        border: 2px solid #1B6E16;
        border-radius: 70px;
        padding: 1rem 3.5rem;
        margin: 10px auto;
    }
    .readmore:hover {
        cursor: pointer;
    }
    .left, .right {
        padding-top: 100px
    }
    .img-col-left {
        text-align: right;
    }
    .row {
        margin-bottom: 5rem;
    }
    .article {
        margin-bottom: 0;
    }
    .article h3 {
        font-size: 30px;
        font-family: "Bodoni MT";
        font-weight: 700;
        margin: 0;
        text-transform: uppercase;
    }
    .article small {
        font-size: 20px;
        font-family: "Now Alt";
        font-weight: 300;
        line-height: 44px;
    }
    .article p, .article li {
        font-size: 20px;
        font-family: "Now Alt";
        line-height: 44px;
    }
    /* Media Queries */
    @media screen and (max-width: 768px) {
        .container {
            width: 80vw;
        }
        .img-col-left img, .img-col-right img {
            width: 100%;
        }
    }
    @media screen and (max-width: 430px) {
        .left, .right {
            padding-top: 30px;
        }
        .page-content h2 {
            font-size: 20px;
        }
        .page-content p {
            font-size: 12px;
            line-height: 30px;
        }
        .container {
            margin-bottom: 0;
        }
        .article h3 {
            font-size: 20px;
            margin-top: 2rem;
        }
        .article small {
            font-size: 15px;
        }
        .article p, .article li {
            font-size: 12px;
            line-height: 24px;
        }
    }
</style>

<div class="page-content">
    <div class="row">
        <div class="col-lg-6 img-col-left order-lg-last">
            <img src="/images/blog/post-1.png" alt="All About Acai">
        </div>
        <div class="col-lg-6 left order-lg-first">
            <div class="container">
                <div class="circle">
              
                </div>
              </div>
            <h2>ALL ABOUT AÇAÍ</h2>
            <p>In case you haven’t been bombarded with enough ads and Instagram posts, acai is a superfood berry that is taking the world by storm. But what exactly is acai berry good for and why should you care?</p>
            <p>In this blog, we’ll give you the low down on nature’s ‘purple gold’, and some uses of acai fruit that can transform your health and wellbeing.</p>
            <button class="readmore" on:click={() => (showModal1 = true)}>Read More</button>
        </div>
    </div>
    <div class="row">
        <div class="col-lg-6 img-col-right">
            <img src="/images/blog/post-2.png" alt="Acai More Than Just a Superfood">
        </div>
        <div class="col-lg-6 right">
            <div class="container inverse">
                <div class="circle inverse">
              
                </div>
              </div>
            <h2>AÇAÍ MORE THAN JUST A SUPERFOOD</h2>
            <p>You may have heard of acai before. It's a superfood that's taken the health industry by storm, and for good reason! Acai berries are packed full of nutrients that have unmatched benefits for your overall health and wellbeing.<br>You might be familiar with acai as a superfood, or as the main ingredient in the trendy acai bowls that are favoured by celebrities around the world. But did you know that there are many different uses for acai?</p>
            <button class="readmore" on:click={() => (showModal2 = true)}>Read More</button>
        </div>
    </div>
    <div class="row">
        <div class="col-lg-6 img-col-left order-lg-last">
            <img src="/images/blog/post-3.png" alt="Reasons Why Acai Is a Superfood">
        </div>
        <div class="col-lg-6 left order-lg-first">
            <div class="container">
                <div class="circle">
              
                </div>
              </div>
            <h2>REASONS WHY AÇAÍ IS A SUPERFOOD</h2>
            <p>Acai berries have been heralded as a superfood for years now. But what exactly makes them so super? And why are they better than other berries, like blueberries or strawberries?</p>
            <p>In this blog, we’re going to explore the reasons why acai is a superfood, and you may be surprised at some of the health benefits! Let's take a closer look at this amazing fruit and find out what all the fuss is about:</p>
            <button class="readmore" on:click={() => (showModal3 = true)}>Read More</button>
        </div>
    </div>
    <div class="row">
        <div class="col-lg-6 img-col-right">
            <img src="/images/blog/post-4.png" alt="Ways you can includ acai into your daily routine">
        </div>
        <div class="col-lg-6 right">
            <div class="container inverse">
                <div class="circle inverse">
              
                </div>
              </div>
            <h2>WAYS YOU CAN INCLUDE AÇAÍ INTO YOUR DAILY ROUTINE</h2>
            <p>Acai is an unlikely superfruit. The acai berry is tiny, jet-black and originates from the swamps of the Amazon. But this little berry has some big health benefits.</p>
            <p>Acai is rich in antioxidants, fibre, and heart-healthy fats. Including acai in your routine can be easy and delicious! Here are some tips on how to get started.</p>
            <button class="readmore" on:click={() => (showModal4 = true)}>Read More</button>
        </div>
    </div>
    <div class="row">
        <div class="col-lg-6 img-col-left order-lg-last">
            <img src="/images/blog/post-5.png" alt="Miracle Berry for Fitness Enthusiast?">
        </div>
        <div class="col-lg-6 left order-lg-first">
            <div class="container">
                <div class="circle">
              
                </div>
              </div>
            <h2>MIRACLE BERRY FOR FITNESS ENTHUSIAST?</h2>
            <p>We’ve all been there. You’re four weeks into your New Year’s resolution of hitting the gym five times a week and you’re already starting to feel the effects of working out that much. You’re sore, you’re tired, and you just don’t have the energy to keep going. But you don’t want to give up on your resolution so soon! What can you do to give yourself a boost?</p>
            <button class="readmore" on:click={() => (showModal5 = true)}>Read More</button>
        </div>
    </div>
</div>

<!-- Modals -->

<Modal bind:showModal1>
    <div class="row article">
        <div class="col-lg-6">
            <h3>What is Acai?</h3>
            <p>Native to the flooded Amazonian forest regions of Brazil, acai berry has been a staple in the diets of indigenous people for centuries. This power-packed fruit has only recently become widely available in North America, but they have already made quite a splash across the world!</p>
            <p>Pronounced “ah-sigh-ee”, these berries are often sold in powder or juice form, and are loaded with more antioxidants than blueberries, cranberries and raspberries! The benefits of acai don’t stop there, they’re also bursting with fibre and heart-healthy fats. So yes, acai is healthy – there’s no doubt about that.</p>
            <p>But here’s the thing – there are plenty of other foods out there that are just as healthy, if not more so. So why all the hype? Why has acai become such a phenomenon? The answer lies in its flavour.<br>Acai has a unique taste that can best be described as a cross between berries and chocolate. It’s rich and creamy, with a slightly sweet taste that is utterly addictive. And once you’ve had it, you’ll understand what all the fuss is about!</p>
            <h3>Health Benefits of Acai</h3>
            <small>But what is acai berry good for?</small>
            <p>As mentioned earlier, acai berries are rich in antioxidants – they’re even referred to as “beauty berries” because of this! Antioxidants are beneficial compounds that scavenge harmful toxins, or free radicals from your body, which can damage cells and lead to inflammation. Free radicals are also responsible for the visible signs of aging - we’re talking wrinkles and fine lines!</p>
            <p>So stock up on acai fruit if you’re looking to combat any tell-tale signs of aging!</p>
            <p>Aside from giving your skin a radiant glow, acai berries are also rich in vitamins A, C, and E as well as calcium and iron. There have also been links between acai berries and weight loss, due to the fruit having appetite suppression qualities – acai berries are rich in fibre, playing a vital role in making sure your digestive system is working as it should.</p>
            <p>In addition to its suggested weight loss benefits, acai berries contain heart-healthy fats. These fruits are rich in oleic acid - a type of monounsaturated fat that has been shown to improve cholesterol levels by reducing LDL cholesterol (the “bad” cholesterol) while increasing HDL cholesterol (the “good” cholesterol). A diet rich in oleic acid has also been <a href="https://cardiab.biomedcentral.com/articles/10.1186/s12933-015-0237-9">linked to a lower risk of stroke and heart disease.</a></p>
        </div>
        <div class="col-lg-6">
            <h3>Uses of Acai</h3>
            <p>Versatile and delicious, the benefits of acai berry can be enjoyed in a range of ways.</p>
            <p>Let’s talk tastebuds - the most common way to take acai, is to consume it! You can eat acai as part of a nourishing smoothie bowl or juice. Due to their slightly sweet taste, acai berries make the perfect ingredient for a ‘superfood smoothie’, especially when blended with nutritious fruits like bananas or strawberries. So if you're looking for a healthy breakfast or snack, a nourishing acai bowl could be just what you need to get your fix of vitamins and nutrients.</p>
            <p>If you're looking for something more unique, you can also find acai oil on the market. Acai oil is said to be good for your skin and hair, as it contains fatty acids that can help moisturize and protect your hair and skin from damage. Believe it or not, but you can even find acai oil in shampoos, conditioners, hair masks, and skin creams!</p>
            <p>For those on the move, acai can also conveniently be found in pill form as a dietary supplement. Similar to the acai berry, acai supplements are said to improve joint function, increase energy levels, reduce inflammation, and promote weight loss.</p>
            <p>Whether you’re looking to take your breakfast to the next level or keep your skin glowing all year round, the benefits of acai are endless.</p>
            <p>There you have it! Acai really is a superfood. It's packed with nutrients that are good for your heart, skin, digestion, and overall health. And as an added bonus, it's a great choice for people who are watching their weight due to its low calorie and sugar content.</p>
            <p>So go ahead and enjoy an acai bowl guilt-free!</p>
        </div>
    </div>
</Modal>

<Modal bind:showModal2>
    <div class="row article">
        <div class="col-lg-6">
            <h3>Nutrients</h3>
            <p>You may have seen acai bowls or acai-based juices and smoothies at your local cafe, but what exactly is this so-called "superfood?"<br>Acai berries are packed full of nutrients. They are an excellent source of vitamin A, vitamin C, and vitamin E, which collectively contribute to:</p>
            <ul>
                <li>Maintaining healthy skin and eyes</li>
                <li>Keeping your immune system in top condition</li>
                <li>Helping wounds heal faster</li>
                <li>Supporting bone health (say goodbye to joint pain!)</li>
            </ul>
            <p>But the benefits of acai don’t stop there, acai berry also contains important minerals like iron and calcium. On top of that, acai berries are rich in antioxidants. In fact, they have one of the highest antioxidant levels of any food on the planet!</p>
            <p>As you may have gathered - acai may be a small fruit, but it packs a big punch when it comes to health benefits. Here are some of the incredible benefits that acai berry has to offer:</p>
            <h3>Acai Berry is Good For Your Skin</h3>
            <p>The benefits of acai berry for skin are endless. That’s because the antioxidant properties of acai berry allow the fruit to protect your skin from damage caused by free radicals. Free radicals are unstable molecules that can cause damage to cells, leading to premature ageing. You know the saying - an acai bowl a day keeps the wrinkles at bay!</p>
            <h3>Acai for Weight Loss</h3>
            <p>If you're looking to shed a few pounds, incorporating acai into your diet may help.</p>
            <p>There isn’t much evidence to support the health claim that acai berry has a particular fat-burning power. However, as part of a balanced diet, acai berry can promote weight loss by increasing feelings of fullness and decreasing appetite due to its high fibre content.</p>
            <p>Eating fibre-dense foods that keep you feeling fuller for longer as they take longer to digest! For example, eating an apple is more filling than drinking apple juice due to the amount of fibre in the raw form.</p>
            <h3>Acai for Heart Health</h3>
            <p>The antioxidants present in acai berries can help protect your heart by reducing inflammation and <a href="https://www.healthline.com/nutrition/13-foods-that-lower-cholesterol-levels">lowering cholesterol levels.</a></p>
            <p>Inflammation is a major risk factor for heart disease, while high cholesterol levels can clog your arteries and lead to a heart attack or stroke. In 2011, a study showed that overweight adults who drank two acai smoothies </p>
        </div>
        <div class="col-lg-6">
            <p>daily had improvements in LDL ("bad") cholesterol levels, compared to those who did not drink the beverage.</p>
            <h3>Acai for Immunity</h3>
            <p>Acai berries are also known for their immune-boosting properties.</p>
            <p>This is thanks to their high content of vitamins A and vitamin C, both of which are essential for a healthy immune system. In addition, acai berries contain flavonoids, which have been shown to increase the production of white blood cells and improve overall immune function.</p>
            <p>So if you're looking for a way to fight off colds and flu this season, look no further than the mighty acai berry!</p>
            <h3>Acai for Brain Function</h3>
            <p>Acai berries are also thought to benefit brain health due to their high antioxidant content.</p>
            <p>Damage caused by free radicals has been linked to age-related cognitive decline. Several studies have proven that the plant compounds in acai have a <a href="https://pubmed.ncbi.nlm.nih.gov/26618555/">‘protective’ effect on the brain,</a> and have also found that acai can improve memory and learning by <a href="https://pubmed.ncbi.nlm.nih.gov/22224493/">counteracting the negative effects of inflammation in brain cells.</a></p>
            <p>Essentially, acai helps to stimulate the brain’s ‘housekeeping’ response, keeping everything in check!</p>
            <h3>Conclusion</h3>
            <p>If you're looking for a delicious way to boost your health, look no further than acai berries.<br>These little purple fruits are not only super tasty but also super nutritious. As we’ve covered, studies have shown that consuming acai can enhance immunity, lower cholesterol levels and protect brain function with age.</p>
            <p>So what are you waiting for? Head to your nearest cafe and order an acai bowl today!</p>
        </div>
    </div>
</Modal>

<Modal bind:showModal3>
    <div class="row article">
        <div class="col-lg-6">
            <h3>Excellent source of fibre</h3>
            <p>Did you know that 70% of your immune system is located in your gut?</p>
            <p>That's why having a healthy gut is so important for overall health. And guess what? Fibre is essential for gut health!</p>
            <p>Fibre feeds the good bacteria in your gut and helps promote the growth of healthy bacteria. This leads to improved gut function and a stronger immune system.<br>So if you're looking to boost your immunity, reach for a fibre-rich acai berry superfood bowl to keep your body in top condition.</p>
            <h3>Rich in Antioxidants</h3>
            <p>Antioxidants are molecules that help your cells by neutralizing free radicals.</p>
            <p>Free radicals are unstable molecules that can damage cells, leading to inflammation. Inflammation is your body’s response to cellular stress or injury and is a major player in the development of chronic diseases like heart disease, Alzheimer’s, and cancer.</p>
            <p>Free radicals are produced when your body breaks down food or is exposed to cigarette smoke, air pollution, or ultraviolet radiation from the sun. The good news is that your body naturally produces antioxidants to keep free radicals in check, but by eating food with a high antioxidant content (such as acai!), you’re giving your system some extra support.</p>
            <h3>Can Help to Lower Cholesterol</h3>
            <p>Another one of the many health benefits of acai is that the fruit contributes to heart health!</p>
            <p>Research has shown that acai berry can keep LDL (the “bad” type of cholesterol) at bay, reducing your risk of clogged arteries and dementia.</p>
            <p>But why is LDL cholesterol bad? Well, it's all about the particles. LDL particles are small and dense, which means they can easily become oxidized and cause inflammation in our arteries. These blockages may result in heart disease or stroke, so minimising this type of cholesterol is essential to keeping your arteries healthy.</p>
            <h3>Can Boost Brain Function</h3>
            <p>Whether you’re a teenager or heading into your 70s, eating foods that boost brain function is always a bonus.</p>
            <p>However, as we age, it’s inevitable that our brains will stop functioning as well as they used to. Luckily, acai has been shown to help prevent ‘cognitive decline by <a href="https://www.betteraging.com/nutrition/can-acai-berries-boost-your-brain-function/">preventing oxidative damage</a> to the proteins and acids in the brain.</p>
            <p>It’s simple – eat acai for better brain function!</p>
            <h3>Can Improve Digestion</h3>
            <p>We've all been there - constipation, bloating, and feeling just overall ‘blah’. Sometimes, no matter how much water we drink or how many prunes we eat, our digestive system just needs a little help. That's where acai comes in. This superfood has been shown to improve digestion and get things moving.</p>
        </div>
        <div class="col-lg-6">
            <p>As mentioned earlier, acai is rich in fibre, which can help to regulate the digestive system and keep things moving smoothly. It also contains compounds that help to reduce inflammation in the gut. This can be helpful for those who suffer from conditions like <a href="https://www.nhs.uk/conditions/crohns-disease/">Crohn's disease</a> or <a href="https://www.nhs.uk/conditions/ulcerative-colitis/">ulcerative colitis.</a></p>
            <p>And it doesn’t stop there - in addition, acai can help to improve gut bacteria levels, which can contribute to overall gut health! Is there anything acai can’t do?</p>
            <h3>Can Help to Promote Skin and Hair</h3>
            <p>There are numerous ways in which acai can benefit your skin and hair!</p>
            <p>First of all, the antioxidants in acai help to protect your skin from damage caused by environmental factors like pollution and UV rays. Additionally, the omega-3 fatty acids present in acai help to keep your skin hydrated and supple.</p>
            <p>Vitamins A, C, and E help to brighten your complexion and give your skin a healthy glow, and also play a role in keeping your hair luxurious! For example, vitamin C is necessary for the production of collagen, which helps to keep your hair follicles strong. Vitamins A and E help to protect your scalp from damage, while iron helps to ensure that your scalp gets enough oxygen-rich blood.</p>
            <p>So if you're looking for a way to give your skin and locks a little boost, adding acai to your diet is a great place to start!</p>
            <h3>Can Help to Reduce Inflammation</h3>
            <p>It’s time to get scientific!</p>
            <p>Acai berries are rich in antioxidants, which are beneficial for reducing inflammation throughout the body, and it’s all down to anthocyanins. These antioxidants help neutralise harmful free radicals in your body.</p>
            <p>If you're looking for ways to reduce inflammation, adding foods like acai berries may be worth considering!</p>
            <h3>Conclusion</h3>
            <p>There's no doubt about it, acai berries are pretty amazing.</p>
            <p>If you're looking for a nutritional powerhouse of a fruit, look no further than the acai berry. Add them to your smoothies, eat them on their own, or enjoy them in one of the many delicious acai bowls that are now available at cafes and restaurants around the world.</p>
            <p>However you choose to eat them, just make sure you do! Your body will thank you for it.</p>
        </div>
    </div>
</Modal>

<Modal bind:showModal4>
    <div class="row article">
        <div class="col-lg-6">
            <h3>Bring Out the Blender</h3>
            <p>Let’s start with our favourite way to eat acai – a ‘superfood’ acai bowl.</p>
            <p>Packed with antioxidants, an acai bowl is perfect for giving your body the nourishment it needs! Making an acai bowl at home is easier than you think!</p>
            <p>All you have to do is blend a thick smoothie using frozen acai, almond milk, and bananas. Pour the mixture into a bowl and top with your favourite toppings, we usually opt for:</p>
            <ul>
                <li>Granola</li>
                <li>Shredded coconut</li>
                <li>Berries</li>
                <li>Kiwi</li>
                <li>Dark chocolate chips</li>
                <li>Nut butters</li>
            </ul>
            <p>Remember, it’s important that you get the health benefits possible from your acai bowl, so make sure to buy quality acai berries from a trusted supplier! Your body will thank you.</p>
            <h3>Time for Tea</h3>
            <p>A warming drink always goes down well in these colder months. Next time you’re needing a winter warmer, pour yourself a mug of acai tea for a nourishing brew that is packed with goodness.</p>
            <p>Most acai berry tea blends tend to be mixed with a green or black tea base. To get the best out of your acai berry brew, invest in a superfood acai powder that you can mix into your favourite milk. Acai powders are also versatile enough to nutritionally enhance smoothies and lattes too!</p>
            <h3>Get Creative in the Kitchen</h3>
            <p>In a world filled with choices, it can be hard to decide what to put on your salad. But don't worry, we're here to help. Give your salads a nutrient boost by using acai as the base for your dressing!</p>
        </div>
        <div class="col-lg-6">
            <p>Simply combine equal parts acai puree with olive oil, apple cider vinegar, and honey (or another sweetener of your choice) in a blender or food processor. Season with salt and pepper to taste.</p>
            <p>The easiness of this recipe isn’t even the best part! Most commercial salad dressings are loaded with sugar, but acai salad dressing is made with all-natural ingredients that are low in sugar. This makes it a great choice for those who are watching their sugar intake or trying to lose weight.</p>
            <p>Gordon Ramsey, eat your heart out!</p>
            <h3>Most Important Meal of the Day</h3>
            <p>Start your day right with a breakfast topper that has antioxidant, anti-inflammatory, antimicrobial and antiviral benefits. That’s right – we’re talking about acai berries!</p>
            <p>Acai makes an undeniably healthy topping for oatmeal or pancakes. Not only are acai berries nutritious and delicious, but they will give you a sustained energy release. Craving something sweet for breakfast but don’t want the rush that comes with added sugars? Top your porridge or pancakes with acai instead of syrup for a healthy alternative.</p>
            <h3>Conclusion</h3>
            <p>There are many different ways you can enjoy the benefits of acai berry, so there's no excuse not to start incorporating it into your daily routine today!<br>Whether you add it to smoothies, make bowls out of it, or just enjoy it as a healthy snack, there's an option for everyone.</p>
            <p>So what are you waiting for? Go forth and get your acai on!</p>
        </div>
    </div>
</Modal>

<Modal bind:showModal5>
    <div class="row article">
        <div class="col-lg-6">
            <h3>Miracle Berry</h3>
            <p>Turns out, there may be a miracle berry that can help. Enter: acai. Native to Central and South America, this small, dark purple berry has been gaining popularity in the fitness world for its supposed health benefits.</p>
            <p>Have we got your attention? Well, here are four reasons why you should consider adding acai to your diet if you’re looking to improve your fitness results. Trust us, you’re going to wish you knew this sooner!</p>
            <h3>Can Help Improve Energy Levels</h3>
            <p>If you’re someone who hits the gym hard, you know that having enough energy is key to maintaining your intensity level and seeing results.</p>
            <p>Unfortunately, it’s not always easy to get all the nutrients you need from your diet alone. That’s where acai comes in.</p>
            <p>Acai berries are home to amino acids that may encourage muscle performance, stamina and strength. This superfood is also loaded with vitamins and minerals that can support the healthy function of the main systems in our body! Because of this, can help give you the boost of energy you need to power through your workouts.</p>
            <p>The benefits of acai really are endless!</p>
            <h3>Can Help Reduce Inflammation</h3>
            <p>Did you know that acai berries contain over 12 times more antioxidants than blueberries?</p>
            <p>Inflammation is a common issue for athletes, particularly if they are training intensely on a regular basis. Acai can help reduce inflammation thanks to its high antioxidant content.</p>
            <p>These antioxidants can help neutralize free radicals that can contribute to inflammation. So, if you’re looking to reduce pain and soreness after your workouts, acai may be able to help.</p>
        </div>
        <div class="col-lg-6">
            <h3>Can Help Improve Recovery Time</h3>
            <p>In addition to reducing inflammation, acai’s high antioxidant content can also help improve recovery time by reducing oxidative stress on cells.</p>
            <p>The simple truth is that your muscles need antioxidants to function properly. Antioxidants help to remove damaged cells and debris that can build up in your muscles after a strenuous workout.</p>
            <p>This means that your muscles will be able to repair themselves more quickly after intense exercise, so you can get back to the gym sooner and see better results in the long run!</p>
            <p>In short, antioxidants are essential for maintaining healthy muscles, and the benefits of acai berry can keep your body topped up with all the good stuff.</p>
            <h3>Can Aid Digestions</h3>
            <p>Acai can also help improve digestion and ‘regularity’! This is especially important if you're someone who works out frequently, as exercise can often lead to digestive issues.<br>But how do acai berries aid digestion? Acai berries are thought to improve digestion by stimulating peristaltic activity – aka “the waves of muscle contraction that push food through your digestive system” - in the intestines. This stimulation helps move food more quickly and efficiently through your system, which can help relieve pesky bowel issues.</p>
            <p>Additionally, the fibre in acai berries can help improve overall gut health… what a bonus!</p>
            <h3>Conclusion</h3>
            <p>As you can see, there are plenty of good reasons to add acai to your diet if you’re a fitness enthusiast.</p>
            <p>If you’re looking for an edge in your workout routine, give this superfood a try and see how it can help you achieve your fitness goals!</p>
        </div>
    </div>
</Modal>