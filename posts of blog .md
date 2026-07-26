# **📖 Blog Order**

## **Phase 1 — Where My AI Journey Started (Bachelor's Thesis)**

### **1\.Why Your Phone Could One Day Detect Skin Cancer Before Your Doctor Does**

### **2\.CNN vs. XGBoost: What I Learned Pitting Deep Learning Against Classic ML for Cancer Detection**

---

## **Phase 2 — Industry Experience (QA Engineer)**

### **3\.From QA Engineer to AI Researcher: How Testing Shaped My Thinking About Model Reliability**

### **4\.The Most Dangerous Bugs Aren't Crashes: What Manual Testing Taught Me About Software Quality**

### **5\.What Being the First QA Engineer on a Product Team Taught Me About Ownership**

### **6\.Why Real Users Never Use Software the Way Developers Expect**

### **7\.Can We Test AI the Way We Test Software? Lessons from My QA Background**

## 

## 

## **Phase 3 — Beginning the Master's Journey**

### **8\.What It's Like to Do a Master's on a Royal Thai Scholarship as a Bangladeshi Student**

**9\.AIT Gives You the Environment—What You Become Is Up to You**  
**10\.Finding Home Away From Home: Everyday Life as an International Student in Thailand**

11\.Seven Days at IETF 122 Bangkok: The Most Inspiring Conference I've Ever Attended

---

## **Phase 4 — Learning the Foundations**

### **12\.What is Federated Learning and Why It's the Future of Privacy-Preserving AI**

### **13\.Graph Neural Networks 101: When Network Structure Actually Matters (And When It Doesn't)**

### **14\.Edge Computing and AI: Why the Future of Intelligence is Local, Not in the Cloud**

---

## **Phase 5 — Master's Thesis Research**

### **15\.What is the Edge-IIoTset Dataset and Why It Matters for Industrial Security Research**

### **16\.Intrusion Detection Systems: The AI Gatekeepers Defending Our Connected World**

### **17\.LoRA in Federated Learning: Can Parameter-Efficient Fine-Tuning Save Edge Devices?**

### **18\.More Complex ≠ Better: The Surprising Truth About Graph Neural Networks for IoT Security**

---

## **Phase 6 — Becoming a Researcher**

### **19\.Occam's Razor in Machine Learning: Why the Simplest Model Often Wins**

### **20\.How I Submitted My First Q1 Journal Paper: A Step-by-Step Guide for New Researchers**

### **21\.Responsible AI: Why Guardrails Matter When Machines Make Decisions About Critical Infrastructure**

---

## **Phase 7 — Exploring New Research Frontiers**

### **22\.Agentic AI Workflows: What Happens When AI Systems Start Making Decisions Autonomously?**

### **23\.Deep Reinforcement Learning Explained: Teaching Machines to Make Smarter Decisions Over Time**

---

## **Phase 8 — Moving Toward Future PhD Interests**

### **24\.Smart Grids 101: How AI is Transforming the Way We Manage Electricity**

### **25\.Federated Learning for Smart Grids: Why Decentralized AI Makes Perfect Sense for Energy Networks**

### **26\.The Privacy Problem in Smart Energy: Why We Can't Just Send Everyone's Power Data to the Cloud**

### **27\.Anomaly Detection in Solar Panels: How Machine Learning Spots Faults Before They Become Failures**

### **28\.Sustainable AI: The Carbon Cost of Training Machine Learning Models (And What We Can Do About It)**

---

## **Phase 9 — Current Chapter**

### **29\.Competing in OpenAI Parameter Golf and LPCVC 2026: What I Learned Entering Global AI Challenges**

This works well as the most recent chapter of your journey.

Phase 1 :**Where My AI Journey Started (Bachelor's Thesis)**

# **Post 1**

## **Why Your Phone Could One Day Detect Skin Cancer Before Your Doctor Does**

A few years ago, if someone had told me that a smartphone might one day help detect skin cancer, I probably would have dismissed it as science fiction.

Today, after spending months researching artificial intelligence for skin lesion analysis, I am no longer so sure.

The idea sounds almost unbelievable.

Imagine noticing a strange mole or skin mark on your arm.

You take a photo.

Within seconds, an AI system highlights whether the lesion appears benign or potentially dangerous and recommends whether you should seek medical attention.

It doesn't replace a doctor.

It doesn't make the final diagnosis.

But it acts as an early warning system.

And when it comes to diseases like skin cancer, early warnings can save lives.

## **The Problem We Don't Talk About Enough**

Skin cancer is one of the most common forms of cancer worldwide.

Like many diseases, its outcome often depends on timing.

When detected early, treatment can be highly effective.

When detected late, the consequences can be devastating.

The challenge is that many skin lesions look remarkably similar.

To an untrained eye, a dangerous melanoma may appear no different from an ordinary mole.

Even trained dermatologists often rely on years of experience, visual examination, dermoscopy, and sometimes biopsies to reach a diagnosis.

This process works.

But it is also time-consuming, expensive, and not equally accessible to everyone.

What happens when there are not enough specialists?

What happens when patients delay seeking medical care?

What happens when early warning signs are overlooked?

These questions motivated my undergraduate thesis.

## **Teaching Machines to See**

Humans learn through experience.

Artificial intelligence learns through data.

For my research, I worked with the HAM10000 dataset, one of the most widely used collections of dermoscopic skin lesion images in medical AI research.

The dataset contains thousands of images representing seven different categories of skin lesions, ranging from common benign conditions to potentially dangerous forms of skin cancer.

The goal was simple:

Could a machine learn to recognize patterns hidden within these images?

Patterns that might help distinguish one type of lesion from another?

Of course, "simple" quickly became complicated.

## **The Messy Reality of Medical Data**

One thing I learned early is that real-world medical data is rarely perfect.

Some lesion categories had thousands of examples.

Others had very few.

This imbalance creates a serious problem.

Imagine trying to teach a student to recognize seven different animals when 80% of the training images contain only cats.

Eventually, the student starts assuming everything is a cat.

Machine learning models behave similarly.

Before training any models, we had to carefully preprocess and balance the dataset to avoid biased learning.

This part wasn't glamorous.

But it was essential.

## **What Surprised Me Most**

When people hear "artificial intelligence," they often imagine something magical.

The reality is far less dramatic.

AI isn't magic.

It's pattern recognition.

The model doesn't understand cancer.

It doesn't understand fear.

It doesn't understand medicine.

It simply learns that certain visual patterns frequently appear together.

Yet somehow, when trained correctly, those patterns can become surprisingly powerful.

In fact, previous studies have shown that deep learning systems can sometimes perform at levels comparable to experienced dermatologists for specific classification tasks.

That realization fascinated me.

Not because AI would replace doctors.

But because it could assist them.

## **The Future in Your Pocket**

Today, AI-assisted medical imaging is already being explored in hospitals, research labs, and healthcare startups around the world.

As smartphone cameras improve and machine learning models become more efficient, it is not difficult to imagine a future where preliminary skin screening becomes available through mobile applications.

There are still challenges.

Accuracy must improve.

Bias must be reduced.

Privacy must be protected.

Medical decisions must remain in human hands.

But the direction is clear.

Healthcare is becoming increasingly data-driven.

## **Looking Back**

My undergraduate thesis began as a machine learning project.

It ended up changing how I think about technology.

For the first time, I saw how artificial intelligence could move beyond recommendation systems, chatbots, and automation.

I saw how it could contribute to something much more meaningful.

Helping detect disease earlier.

Helping doctors work more efficiently.

Helping patients receive care sooner.

Maybe one day your phone won't diagnose skin cancer.

But it might help ensure that dangerous symptoms are noticed before it's too late.

And that possibility alone makes this field worth exploring.

---

# **Post 2**

## **CNN vs. XGBoost: What I Learned Pitting Deep Learning Against Classic ML for Cancer Detection**

When people talk about artificial intelligence today, deep learning usually steals the spotlight.

Convolutional Neural Networks.

Transformers.

Foundation models.

Massive GPU clusters.

It's easy to assume that traditional machine learning methods have become obsolete.

During my undergraduate thesis, I decided to test that assumption.

What happens when a custom deep learning model goes head-to-head against classic machine learning algorithms on the same skin cancer classification task?

The answer surprised me.

## **The Setup**

The project focused on classifying seven categories of skin lesions using the HAM10000 dataset.

Instead of relying on a single approach, I built two separate pipelines.

### **Approach 1: Deep Learning**

A custom Convolutional Neural Network (CNN) trained directly on skin lesion images.

The CNN learned visual patterns automatically from the data.

No manual feature engineering.

No handcrafted rules.

Just images and learning.

### **Approach 2: Traditional Machine Learning**

For the second approach, I used a CNN as a feature extractor and then fed those extracted features into several machine learning classifiers, including:

* XGBoost  
* Random Forest  
* Support Vector Machine  
* Logistic Regression  
* KNN  
* Decision Tree

The idea was simple:

Could traditional classifiers compete if they were given high-quality image features?

## **The Assumption I Started With**

Like many students entering AI research, I assumed deep learning would win.

After all, most modern breakthroughs in computer vision come from neural networks.

But I expected the margin to be enormous.

I thought traditional machine learning would struggle.

I was wrong.

## **The Results**

The customized CNN achieved approximately 80% classification accuracy.

The best-performing traditional machine learning model was XGBoost, achieving approximately 77% accuracy.

Three percentage points.

That's all.

After weeks of experimentation, preprocessing, balancing, tuning, and debugging, the gap between the two approaches was surprisingly small.

That result forced me to rethink some assumptions.

## **The Lesson Nobody Talks About**

In AI communities, there is often an obsession with using the newest and most complex model.

Bigger networks.More layers.More parameters.More computation.

But complexity does not automatically guarantee dramatically better performance.

In this project, traditional machine learning remained remarkably competitive.

Why?

Because good features matter.Clean data matters.Preprocessing matters.

Problem formulation matters.

Sometimes those factors matter more than the choice of algorithm itself.

## **The Hidden Challenge: Data**

The biggest obstacle wasn't choosing CNN or XGBoost.

The biggest obstacle was the dataset.

The HAM10000 dataset contains multiple lesion categories, but the distribution is highly imbalanced. Some classes contain significantly more samples than others.

Without proper balancing, models naturally become biased toward the dominant classes.

Much of the project involved:

* Resizing images  
* Encoding labels  
* Balancing classes  
* Splitting datasets  
* Testing different hyperparameters

In many ways, data preparation required more effort than model training.

## **A Lesson That Followed Me Into Graduate Research**

Looking back, this undergraduate project taught me something that would later reappear during my Master's research.

The best-performing solution is not always the most sophisticated one.

Researchers often fall into the trap of chasing complexity.

But sometimes simpler approaches perform surprisingly well.

Sometimes they are easier to deploy.

Sometimes they are more interpretable.

And sometimes they win.

That lesson eventually influenced how I approached later research involving Federated Learning, Graph Neural Networks, and IoT security.

## **Final Thoughts**

If I had to summarize the project in one sentence, it would be this:

> Deep learning won the competition—but traditional machine learning refused to lose.

The CNN achieved the highest accuracy, but XGBoost came remarkably close.

More importantly, the project taught me that machine learning is not about finding the most complex model.

It is about understanding the problem, understanding the data, and choosing the right tool for the job.

That lesson has stayed with me far longer than any accuracy score ever could.

PHASE 2 : 

## **3\. From QA Engineer to AI Researcher: How Testing Shaped My Thinking About Model Reliability**

My first real job as a QA engineer didn’t feel glamorous at all. I wasn’t “building cool features” or “designing architectures.” I was the person who clicked the same button twenty times from twenty different angles, late into the evening, just to see if it would break. Some days I went home with nothing to show except a list of bugs in a spreadsheet and a tired pair of eyes.

But something important was happening in those quiet hours. I started to see patterns—how small misunderstandings in requirements turned into confusing screens, how a “tiny” UI inconsistency could make users doubt the whole product, how one unnoticed edge case could ruin someone’s day. I realized my job wasn’t to be the person who breaks things. I was the person who protects the user’s trust, even when they never know I existed.

That mindset followed me when I moved into AI and research. Today, when I train a model, I don’t just look at the accuracy number and feel satisfied. The old QA part of me asks: *What happens on the weird inputs? On data we didn’t expect? On that one rare class that only appears a few times?* Reliability, to me, is no longer just “passes the test suite” or “hits 95 percent.” It means: *Can this system behave in a stable, understandable way when the world is messy—because it always is?*

Looking back, my QA job was my first real lesson in humility. The software never behaved exactly how the developers imagined, and neither do machine learning models. Both will surprise you, and not always in a good way. Learning to anticipate those surprises—patiently, carefully, and sometimes painfully—is what quietly prepared me for the kind of research I do now.

---

## **4\. The Most Dangerous Bugs Aren’t Crashes: What Manual Testing Taught Me About Software Quality**

In my first months as a manual tester, I secretly liked crashes. When a feature crashed, at least it was obvious. I could take a screenshot, log the steps, attach the error message, and feel that satisfying “Bug Report Submitted” moment. It was clean. Clear. Undeniable.

The bugs that scared me most were the silent ones—the ones where everything *looked* fine. The page loaded. The button worked. The numbers were there. But something in my gut said, “This isn’t right.” Maybe a total was slightly off. Maybe a date was misinterpreted. Maybe the app allowed something it should have rejected. There was no explosion, no dramatic error. Just small, quiet wrongness that might never be noticed until it hurt someone.

Hunting those bugs taught me what “quality” really means. It’s not just “the app doesn’t crash.” It’s:

* Does this behave the way a user would *naturally* expect?  
* Are we giving the right information, not just *some* information?  
* Will this still make sense when the user is tired, stressed, or in a hurry?

As I moved toward AI work and my master’s research, this lesson became even sharper. A model that fails loudly is actually easier to fix. The dangerous ones are models that seem to perform well overall but quietly discriminate against a subgroup, or fail on an important edge case, or give confidently wrong answers in rare but critical situations. You don’t see these failures if you only stare at one big metric.

Manual testing forced me to develop a kind of emotional radar for “something feels off.” It’s not scientific by itself, but it pushes me to dig deeper, design better checks, and never be satisfied with “it didn’t crash, so it’s fine.” That instinct is still one of my most valuable skills, even in the world of AI.

---

## **5\. What Being the First QA Engineer on a Product Team Taught Me About Ownership**

Starting as the first QA engineer on a product team felt a bit like walking into a house that everyone was already living in—but nobody had ever checked the foundation. Features were shipping. Customers were using the product. Developers were moving fast. But there was no test plan, no clear process, and no one whose job it was to say, “Wait, is this actually ready?”

In the beginning I felt small. I was the youngest person in the room, with the least experience. Who was I to question a senior developer’s work or ask a product manager to clarify a requirement? But every time a user reported a bug we *could* have caught earlier, it felt like a personal failure—even if nobody blamed me. Slowly, I realized something: if I didn’t take ownership of quality, nobody else would.

So I started small. I kept my own checklists. I wrote simple test cases in a spreadsheet. I politely pushed back when timelines were unrealistic. I learned to say, “If we skip testing this part, here is what might happen to the user.” At first, it was uncomfortable. My hands literally shook the first few times I disagreed in a meeting. But over time, people started to listen. Developers asked me to review things earlier. Product managers came to me with questions about edge cases. The role I thought was “just testing” slowly became “guarding the product.”

That experience changed how I see my work today. As a researcher, it’s easy to think our job ends at “finishing the experiment” or “writing the paper.” But being that first QA taught me a different definition of ownership: you are responsible not just for your task, but for the impact of your work on real people. When I design a model or evaluate a system now, I feel that same sense of responsibility I felt when I signed off a build. It’s not just code. It’s something someone will rely on.

---

## **6\. Why Real Users Never Use Software the Way Developers Expect**

One of the funniest parts of being a QA engineer is realizing just how creative real users are—without even trying. Developers would explain a feature to me, and it always sounded so neat and linear: “The user will do A, then B, then C.” Then we would launch it, and users would do Z, skip B entirely, and try to drag C onto A.

In testing, I started playing a little game with myself: *If I were completely new, late for work, half‑distracted, and slightly annoyed… what would I click?* That simple shift changed everything. I typed things in the “wrong” format. I went back and forth between pages. I double‑clicked buttons that were meant for single clicks. And sure enough, that’s where the weird behavior and hidden bugs lived.

Those moments made me more empathetic. Most users are not “doing it wrong”; they are doing it in the most human way they can, given their context. They are tired, busy, sometimes scared of technology, sometimes overconfident. Software doesn’t live in a perfect tutorial. It lives in messy human lives.

Now, in AI and research, I carry that same question with me: *How will people actually interact with this system?* A model that works beautifully in a controlled experiment might behave very differently when real data comes in out of distribution, or when users misunderstand instructions, or when the environment changes. Real users will never “follow the script,” and honestly, they shouldn’t have to. It’s our job—as testers, engineers, and researchers—to design for how people really behave, not how we wish they would.

---

## **7\. Can We Test AI the Way We Test Software? Lessons from My QA Background**

When I first stepped from traditional QA into the world of AI, I secretly hoped I could treat models like any other feature: write test cases, define expected outputs, and tick boxes. Very quickly, I learned it wasn’t that simple. A login form either accepts a correct password or it doesn’t. But an AI model can be “a little bit wrong” in a thousand different ways.

Still, my QA background refused to stay quiet. I found myself asking familiar questions in a new context:

* What are the obvious happy paths we’re testing?  
* What edge cases are we ignoring?  
* Have we tried “breaking” this model the way we tried breaking that UI?

Of course, you can’t unit test every possible input to an AI model. But you *can* carry over the mindset: be suspicious of averages, design stress tests, and care deeply about rare but high‑impact failures. Instead of just checking if the model performs well on the test set, I started thinking like a tester again: *Where is this model most fragile? If I were a malicious user, how would I try to confuse it? If I were a non‑technical user, how might I misunderstand its output?*

The honest answer to “Can we test AI the way we test software?” is: not exactly. But we can—and should—bring the discipline and empathy of QA into AI evaluation. My year in QA taught me to see beyond green checkmarks and passing builds. It taught me to listen for the quiet failures, worry about the user who can’t file a ticket, and question “good enough” results. In a world where AI systems increasingly affect real people and critical infrastructure, those lessons matter more than ever.

## **Phase 3 — Beginning the Master's Journey**

# **What It's Like to Do a Master's on a Royal Thai Scholarship as a Bangladeshi Student**

There are moments in life that quietly divide everything into a "before" and an "after."

For me, one of those moments arrived in the form of an email.

I had been accepted to pursue a Master's degree in Information and Communication Technologies at the Asian Institute of Technology (AIT) in Thailand under the King's Scholarship.

At the time, I understood that it was a great opportunity. What I didn't realize was how profoundly it would change the course of my life.

## **A Dream That Felt Far Away**

Like many students from Bangladesh, I had always wanted to study abroad.

Not because I wanted to leave home permanently.

Not because I thought opportunities elsewhere were magically better.

But because I wanted to experience a different academic environment, meet people from around the world, and challenge myself beyond what was familiar.

The problem, of course, was money.

Anyone who has looked into international education knows that tuition fees alone can be overwhelming. Then come accommodation costs, registration fees, health insurance, travel expenses, and countless other expenses that quietly accumulate.

For many students, the dream of studying abroad ends before it even begins.

The King's Scholarship changed that.

## **More Than Financial Support**

When people hear the word "scholarship," they often think only about money.

But what the scholarship gave me was much more than financial support.

It gave me freedom.

Freedom to choose courses based on what interested me rather than what seemed financially practical.

Freedom to focus on research instead of constantly calculating expenses.

Freedom to attend seminars, workshops, competitions, and conferences without feeling guilty about every small expenditure.

Freedom to invest my energy in learning.

For the first time, I could truly focus on becoming a student.

## **The Journey to Thailand**

My journey to Thailand wasn't perfectly smooth.

There were visa procedures, paperwork, preparations, and a hundred little details that needed attention.

When the day finally arrived, I boarded a plane carrying more than luggage.

I carried excitement.

I carried uncertainty.

I carried expectations.

And if I'm being honest, I carried a little fear too.

I was leaving behind familiar streets, familiar food, familiar people, and stepping into a completely new chapter.

When I landed at Suvarnabhumi Airport, I remember standing there with my bags, surrounded by people speaking different languages, all moving confidently toward destinations they already knew.

I was different.

I had never navigated this journey before.

There was no family member waiting outside.

No one to guide me step by step.

Just me, a phone, some directions, and a destination called AIT.

Looking back now, that small journey from the airport to campus feels symbolic.

It was my first lesson in independence.

## **Arriving at AIT**

As I entered the campus, I remember being struck by how green everything looked.

The roads were lined with trees.

The air felt calmer than the busy city outside.

Students from different countries walked around speaking different languages.

For the first time, I was living in a truly international environment.

At that moment, AIT felt enormous.

Not just physically.

Emotionally.

There were so many new experiences waiting ahead that I couldn't possibly imagine them all.

## **Learning Beyond the Classroom**

People often assume a Master's degree is mostly about classes and research.

In reality, some of the most important lessons happen outside the classroom.

Living abroad forced me to learn things I had never seriously thought about before.

How to manage money.

How to budget for a month.

How to complete administrative paperwork.

How to open a bank account.

How to navigate a healthcare system.

How to solve problems when there is no immediate support system around you.

Each challenge felt small individually.

Together, they transformed me.

## **Opportunities Beyond Academics**

One of the greatest gifts of the scholarship was the ability to explore opportunities beyond coursework.

At AIT, there was always something happening.

A seminar.

A workshop.

A guest lecture.

A conference.

A competition.

A networking event.

Researchers from around the world regularly visited campus.

Industry professionals shared their experiences.

Experts discussed emerging technologies.

Some events were directly related to my research.

Others were completely outside my field.

Yet every one of them expanded my perspective.

Education, I realized, happens everywhere—not only inside classrooms.

## **Travel, Discovery, and Growth**

Living in Thailand also gave me opportunities to explore places I had only seen in photographs.

Weekend trips.

Visits to different cities.

Experiencing local culture.

Trying new food.

Learning how people live in different regions.

These experiences may not appear on a transcript, but they became an important part of my education.

Travel teaches curiosity.

Curiosity fuels learning.

And learning shapes growth.

## **Looking Back**

When people ask me what the King's Scholarship gave me, my answer is simple.

It gave me space to grow.

It allowed me to pursue a Master's degree without carrying the heavy burden of tuition fees and registration costs.

It allowed me to focus on becoming a better researcher, a better student, and ultimately a more independent person.

The degree itself is valuable.

The research experience is valuable.

But perhaps the most important thing I gained was confidence.

Confidence that I could move to a new country.

Confidence that I could adapt.

Confidence that I could build a life far from home.

Years from now, when I look back on this chapter of my life, I know I won't remember only the courses I took or the grades I received.

I'll remember the opportunity that changed everything.

And I'll always be grateful for it.

# **AIT Gives You the Environment—What You Become Is Up to You**

One of the biggest misconceptions people have about universities is that they believe a university can transform them.

After spending nearly two years at AIT, I have come to believe something slightly different.

A university can provide opportunities.

A university can provide resources.

A university can provide an environment.

But what you ultimately become depends on what you choose to do with those opportunities.

And AIT, perhaps more than any place I have experienced, gives you plenty of them.

## **The First Morning**

I still remember some of my first mornings on campus.

Coming from a crowded city environment, the silence felt unusual.

The roads were lined with trees.

The campus stretched far beyond what I initially expected.

Students walked or cycled to class.

Birds could be heard in the background.

For a moment, it was easy to forget that one of Thailand's busiest cities was only a short distance away.

There was something calming about the place.

Something that quietly encouraged you to focus.

At the time, I didn't realize how valuable that environment would become.

## **A Campus Designed for Growth**

One thing I quickly learned about AIT is that almost everything a student needs is within reach.

If you want to stay active, there is a spacious gym.

There are football fields where students gather in the evenings.

Basketball courts filled with friendly competition.

Tennis courts.

Multiple badminton courts.

Jogging routes.

Open spaces to walk after a long day of classes.

Some of my clearest thoughts about research problems came not while sitting in front of a laptop, but while walking around campus.

Sometimes all you need is movement and fresh air.

And AIT gives you plenty of both.

## **Convenience You Learn to Appreciate**

As an international student, daily life matters.

Much more than people realize.

At first, everything feels unfamiliar.

Where do you buy groceries?

Which stores are affordable?

Where can you find ingredients that remind you of home?

Over time, these questions find answers.

The grocery stores near campus carry many South Asian ingredients that I never expected to find in Thailand.

Many of the spices I grew up with were available.

There was affordable food around campus.

A 7-Eleven right inside the university.

Food stalls.

Small restaurants.

Convenience stores.

Everything needed for daily life.

When deadlines are approaching and assignments are piling up, these little conveniences make a bigger difference than people imagine.

## **Safety Creates Freedom**

One thing I rarely appreciated enough until later was how safe the campus felt.

Security operates around the clock.

Students walk around at all hours.

Research often extends late into the night.

Group meetings happen after dinner.

Sometimes you leave the lab when most of the world is already asleep.

Knowing that the campus remains secure allows students to focus on their work rather than worrying about their surroundings.

That sense of security creates freedom.

Freedom to learn.

Freedom to explore.

Freedom to grow.

## **Beyond the Gates**

One of the things I loved most was that AIT never felt isolated.

Just outside campus lies an entire ecosystem.

Nearby markets.

Hospitals.

Hair salons.

Massage centers.

Cafes.

Street food vendors.

Restaurants.

Local shops.

The beautiful Thammasat University Rangsit Campus area nearby adds even more opportunities for students to explore.

And when you want to visit Bangkok, transportation is relatively straightforward.

You can spend the week focused on research and then spend a weekend exploring one of Southeast Asia's most vibrant cities.

Few places offer that balance so naturally.

## **Opportunities Are Everywhere**

What surprised me most wasn't the campus itself.

It was the constant stream of opportunities.

Every week, it seemed like there was another seminar.

Another workshop.

Another guest lecture.

Another networking event.

Another research talk.

Sometimes the topic had nothing to do with my field.

But I attended anyway.

And often those sessions ended up teaching me something unexpected.

One of the most valuable lessons I learned at AIT is that growth often happens outside your comfort zone.

The seminar you almost skipped.

The workshop you attended out of curiosity.

The competition you weren't sure you were qualified for.

Those experiences often become the most memorable ones.

## **Two Students, Same Campus**

Over time, I noticed something interesting.

Two students could spend the same two years at AIT and leave with completely different outcomes.

They attended the same university.

Used the same facilities.

Walked the same roads.

Had access to the same professors.

Lived on the same campus.

Yet one student leaves with publications, professional connections, research experience, lifelong friendships, and confidence.

The other leaves wondering where the time went.

The difference is rarely intelligence.

More often, it is initiative.

AIT opens doors.

You still have to walk through them.

## **The Golden Years**

Looking back now, I realize how easy it is to underestimate this period of life while living through it.

Assignments feel stressful.

Research deadlines feel overwhelming.

Administrative paperwork feels annoying.

But one day, it all becomes a memory.

The conversations after class.

The spontaneous tea breaks.

The football matches.

The late-night project discussions.

The seminars.

The friendships.

The opportunities.

These years pass much faster than we expect.

And once they are gone, they do not return.

## **What AIT Really Gives You**

When people ask me about AIT, they often ask about rankings, programs, professors, or facilities.

Those things matter.

But they are not what I remember most.

What I remember is the environment.

An environment where students from dozens of countries live together.

An environment that encourages curiosity.

An environment filled with opportunities waiting to be discovered.

An environment that quietly challenges you to become a better version of yourself.

AIT gives you the environment.

What you become is up to you.

And if there is one lesson I would share with every new student arriving on campus, it is this:

Take the opportunities.

Attend the seminar.

Join the competition.

Talk to the professor.

Meet new people.

Explore new ideas.

Because one day, when you look back on your time here, you will realize that these were not just university years.

They were some of the most important years of your life.

# **Finding Home Away From Home: Everyday Life as an International Student in Thailand**

When people think about studying abroad, they often imagine classrooms, research papers, presentations, and graduation photos.

What they don't see are the small moments in between.

The moments that slowly turn a foreign country into a second home.

When I first arrived in Thailand, everything felt unfamiliar. The language was different. The transportation system was different. Even simple tasks like grocery shopping seemed more complicated than they should have been.

For the first time in my life, I had to handle everything on my own.

I still remember arriving at Suvarnabhumi Airport with my luggage and trying to figure out how to reach AIT. It wasn't a dramatic journey, but it was the beginning of something new. Every step required a decision. Every decision required confidence.

Once I arrived at AIT, another challenge began: building a life.

There was paperwork to complete.

Visa requirements to understand.

Documents to submit.

A bank account to open.

As an international student, these things suddenly become your responsibility.

Thankfully, I wasn't alone.

One of our community leaders and his wife generously helped me navigate the process of opening a bank account. What seemed confusing at first became manageable because someone took the time to guide me.

That experience taught me something important: independence does not mean doing everything alone. Sometimes it means knowing when to ask for help.

Then came another challenge: food.

Before moving to Thailand, I had never really cooked.

At first, I relied on campus food and nearby restaurants. But over time, I started learning where to buy groceries, which stores offered the best prices, and where I could find ingredients that reminded me of home.

Eventually, I started cooking.

My early attempts were far from perfect.

Some meals were too salty.

Some were too spicy.

Some were barely edible.

But little by little, I improved.

Today, cooking has become one of those skills I never expected to learn through a Master's degree.

Living abroad also taught me how to manage money.

When you are responsible for your own expenses, you begin paying attention to things you never noticed before.

You learn the difference between wants and needs.

You learn to plan.

You learn to budget.

And perhaps most importantly, you learn how much effort goes into maintaining a comfortable life.

Yet some of my favorite memories are not connected to academics, finances, or responsibilities.

They are connected to people.

One of the funniest examples involves parcel deliveries.

Like many students, I ordered things online from time to time. Unfortunately, I also had a habit of missing phone calls from the delivery service.

One day, when I finally went to collect a package, the J\&T delivery staff member looked at me and immediately asked why I never answered my phone.

I couldn't help but laugh.

From then on, we recognized each other whenever I came to collect a parcel.

We never exchanged names.

We never had long conversations.

Yet somehow we became familiar faces in each other's routines.

Later, I learned that she was a university graduate herself, working hard every day with a smile that never seemed to disappear.

That interaction stayed with me because it reminded me how many hardworking people quietly help make our daily lives easier.

Looking back now, I realize that my experience in Thailand was about much more than earning a degree.

It was about learning how to build a life from scratch.

How to adapt.

How to be independent.

How to ask for help.

How to cook.

How to manage money.

How to find comfort in unfamiliar places.

And somewhere along the way, Thailand stopped feeling foreign.

It started feeling like home.

# **Seven Days at IETF 122 Bangkok: The Most Inspiring Conference I've Ever Attended**

Before attending IETF 122 in Bangkok, I knew what the Internet was.

After attending IETF 122, I began to appreciate how much work happens behind the scenes to keep the Internet running.

For seven days, I had the opportunity to attend the Internet Engineering Task Force (IETF) 122 meeting in Bangkok alongside my friend, Inisha Pradhan.

The conference was held at the beautiful Marriott Marquis hotel, and from the moment I arrived, I could feel that this was not an ordinary event.

Every hallway was filled with conversations.

Every meeting room was filled with experts discussing ideas.

Every corner seemed to contain people solving problems that would eventually affect millions—or even billions—of Internet users around the world.

What made the experience even more special was that we were among the first students sponsored through the I/O Foundation initiative.

As students, it was difficult not to feel a little intimidated at first.

Many attendees had decades of experience.

Some had helped develop technologies and standards that people use every day without even realizing it.

Yet what surprised me most was how welcoming the community was.

People were willing to explain concepts.

Share experiences.

Answer questions.

And encourage newcomers to participate.

One of my favorite parts of the conference was simply moving from room to room.

Every session introduced a different challenge, a different perspective, and a different group of experts.

Some discussions focused on technical protocols.

Others focused on security, privacy, and the future of Internet infrastructure.

What impressed me most was seeing how collaborative the process was.

The Internet is often perceived as something that simply exists.

But behind every standard and every protocol are countless discussions, debates, and contributions from people around the world working together.

The conference also reminded me how large the research community truly is.

As students, it is easy to spend most of our time within our university, department, or research group.

At IETF, I was suddenly surrounded by people from industry, academia, government organizations, and technology companies from across the globe.

It was inspiring.

It was humbling.

And it was motivating.

By the end of the week, I left with far more than technical knowledge.

I left with a broader perspective on collaboration, research, and innovation.

I left with new connections.

New ideas.

And a renewed excitement for the future.

For anyone considering attending an international conference, my advice is simple: go if you have the opportunity.

The presentations are valuable.

The technical sessions are valuable.

But sometimes the most important thing you gain is the realization that you are part of a much larger community of people who are all trying to build something better.

For me, IETF 122 was not just a conference.

It was a glimpse into how the future of the Internet is shaped—and an experience I will never forget.

**Phase 4**

## **12\. What is Federated Learning and Why It’s the Future of Privacy-Preserving AI**

I discovered federated learning the way many students discover life‑changing ideas: by accident while looking for “some privacy‑preserving method” for a project. At first, it sounded almost magical—*train on many devices without ever collecting their data centrally*. The more I read, the more it felt like the missing piece for everything I cared about: IoT, security, and real‑world constraints.

Traditional machine learning has a bad habit: it wants all your data in one place. Every photo, sensor reading, and log line gets shipped to a central server so a model can be trained. That’s powerful, but risky and often incompatible with privacy laws, user expectations, and bandwidth limits. **Federated learning (FL)** flips this pattern. Instead of moving data to the model, we move the **model to the data**.

In FL, a central server initializes a global model and sends it to many clients—phones, hospitals, factories, or edge devices. Each client trains the model locally on its own data, then sends back only **model updates**, not raw records. The server aggregates these updates into an improved global model and redistributes it, repeating this until convergence. This brings several important benefits:

* **Privacy** – Raw data never leaves the device or organization; only learned parameters do, which is crucial for sensitive domains like healthcare, finance, and critical infrastructure.  
* **Lower bandwidth** – Clients send compact updates instead of streaming gigabytes of logs, reducing network and cloud costs.  
* **Personalization** – Different clients can adapt a shared model to their own local patterns while still contributing to a global model.

Working on federated intrusion detection for Edge‑IIoTset made all of this feel very concrete for me. I wasn’t just reading about FL anymore—I was watching how non‑IID data, unstable clients, and edge constraints made the problem messy and interesting. FL is not magic; it still faces challenges like heterogeneous data, communication overhead, and possible leakage through gradients, which is why techniques like differential privacy and secure aggregation are so important. But as our data becomes more distributed and more sensitive, federated learning feels less like an option and more like a blueprint for how serious AI will have to work.

---

## **13\. Graph Neural Networks 101: When Network Structure Actually Matters (And When It Doesn’t)**

My first encounter with Graph Neural Networks (GNNs) was through a paper with intimidating formulas and beautiful diagrams. The idea that you could learn directly on **graphs**—social networks, molecules, power grids—felt like unlocking a hidden “third dimension” of data that standard models never see. As someone interested in networks and IoT, I was instantly hooked: *finally, a model that understands connections, not just isolated rows.*

Most beginner ML models treat data as independent points: each sample is a row in a table or a pixel grid in an image. But many real‑world problems are about **relationships**—who talks to whom, which devices connect, which users are linked, which nodes are neighbors in a grid. GNNs are built for this. In a graph, we have **nodes** (entities) and **edges** (relationships), sometimes with extra features on both. GNNs follow a “message passing” pattern: at each layer, every node aggregates information from its neighbors and updates its own representation. After several layers, a node’s embedding encodes both its own features and the structure around it.

This makes GNNs powerful for tasks like node classification (fraud detection on transaction graphs), link prediction (friend or product recommendations), and graph classification (predicting properties of molecules or materials). They shine when **network structure carries real signal**—for example:

* Social and recommendation graphs, where connections encode influence or similarity.  
* Knowledge graphs, where edges represent semantic relationships.  
* Physical and cyber‑physical systems (power grids, communication networks, transportation) where topology affects flow and behavior.

But my thesis taught me an important “reality check.” On Edge‑IIoTset, the data I worked with was primarily **tabular network traffic features**, not an explicit physical graph with clear, meaningful edges. We still explored spatio‑temporal GNNs under federated constraints, but the results were more nuanced than “GNNs always win”—in some settings, simpler architectures performed competitively or better, especially when we considered latency, memory, and communication limits at the edge.

So here’s my current view: GNNs are amazing when the graph is real, interpretable, and truly relevant to the task. When your “graph” is just a convenience or a weak proxy, the extra complexity may not pay off. That’s a humbling lesson, but also a helpful one: use GNNs when structure really matters; don’t force everything into a graph just because it’s fashionable.

---

## **14\. Edge Computing and AI: Why the Future of Intelligence is Local, Not in the Cloud**

The first time I deployed a model on a small device and saw it make predictions **without** sending data to the cloud, it felt strangely powerful. No big GPU cluster, no long network path—just a modest edge node quietly doing its job. Coming from IoT security and federated learning, that moment made something click: maybe the future of AI isn’t just “bigger models in bigger clouds,” but *smarter models closer to where things actually happen*.

For years, the main pattern was: collect data at the edge, send it to the cloud, run heavy models there, and send results back. That works, but as devices explode in number and data volumes grow, we hit limits. Latency becomes an issue (you can’t wait for the cloud to brake a car or stop a machine), bandwidth gets expensive, and sending sensitive data across networks raises privacy and regulatory concerns.

**Edge computing** changes the emphasis. Instead of doing all intelligence in distant data centers, we run models **close to where data is generated**—on gateways, base stations, industrial controllers, or even directly on IoT devices. This brings several big advantages:

* **Low latency** – Decisions happen in milliseconds because data stays local. This is crucial in industrial automation, autonomous systems, and real‑time monitoring.  
* **Better privacy and security** – Sensitive data doesn’t have to leave the site; only aggregated or anonymized information may go upstream.  
* **Reduced bandwidth and cost** – Local processing means less raw data flowing over networks and less dependence on cloud compute.  
* **Resilience** – Edge systems can keep working even with poor or intermittent connectivity, which is essential for remote or mission‑critical environments.

Recent advances in compact models, quantization, accelerators (TPUs, NPUs, Jetson‑class devices), and lightweight runtimes are making edge AI much more practical. The emerging reality is a **hybrid architecture**: the cloud handles heavy training and global coordination, while the edge focuses on fast, context‑aware inference and sometimes local fine‑tuning.

For my own work—federated learning and IoT intrusion detection on datasets like Edge‑IIoTset—edge computing isn’t an abstract concept. It defines the constraints: limited CPU, memory, energy, and bandwidth, but high expectations for reliability and security. That’s why I’m so interested in models and frameworks that respect these constraints. If AI is going to protect smart grids, factories, and critical infrastructure, it can’t live only in a cloud dashboard. It has to live where the data and the decisions are: at the edge.

## **Phase 5 — Master's Thesis Research**

## **15\. What is the Edge-IIoTset Dataset and Why It Matters for Industrial Security Research**

The first time I opened the Edge‑IIoTset CSV, my laptop fan started screaming. Millions of rows. Dozens of features. It felt less like a “dataset” and more like someone had poured an entire industrial network into a spreadsheet. But hidden in that chaos is exactly what makes Edge‑IIoTset special.\[[kaggle](https://www.kaggle.com/datasets/sibasispradhan/edge-iiotset-dataset)\]

Edge‑IIoTset is a large, realistic cybersecurity dataset built for **IoT and Industrial IoT (IIoT)** scenarios. It combines traffic from more than ten types of devices—sensors, actuators, controllers, and other industrial components—along with a wide variety of attacks, from brute‑force and password guessing to scanning, spoofing, ransomware, and DDoS. Instead of focusing only on one lab setup, it aims to capture how real edge and industrial environments behave when they are both healthy and under attack, which makes it ideal for training and benchmarking intrusion detection systems in modern IIoT networks.\[[ieeexplore.ieee](https://ieeexplore.ieee.org/document/9751703/)\]

Technically, the “DNN‑EdgeIIoT‑dataset” version alone contains over **2.2 million records** and around **63 features**, ranging from network‑level attributes (IP addresses, ports, protocol flags) to higher‑level indicators. The class distribution is heavily imbalanced, with a large share of “Normal” traffic and a smaller but rich variety of attack samples—just like real networks, where attacks are rare but critical. For researchers, this imbalance is both a headache and a gift: it forces models to deal with reality instead of clean, perfectly balanced toy datasets.\[[github](https://github.com/nickjeffrey/ensemble_learning/blob/main/Edge-IIoTset2023_dataset_preprocessing.md)\]

In my thesis, Edge‑IIoTset was the backbone of a federated benchmarking framework for intrusion detection at the edge. Because the dataset is so comprehensive, I could systematically compare simple models (like MLPs) with complex spatio‑temporal GNNs under realistic constraints, instead of relying on small, outdated benchmarks. If you care about industrial security, Edge‑IIoTset isn’t just “another dataset”—it’s a playground where you can stress‑test your ideas against messy, modern reality.\[[emergentmind](https://www.emergentmind.com/topics/edge-iiotset-dataset)\]

---

## **16\. Intrusion Detection Systems: The AI Gatekeepers Defending Our Connected World**

If you imagine a modern factory, power plant, or smart building, it’s not just machines and cables anymore—it’s a dense network of computers, sensors, PLCs, and IoT devices quietly talking to each other. Somewhere in that chatter, an attacker might be scanning ports, injecting malicious packets, or trying to take over a controller. **Intrusion Detection Systems (IDS)** are the gatekeepers watching this traffic.\[[fortinet](https://www.fortinet.com/resources/cyberglossary/intrusion-detection-system)\]

At a high level, an IDS is a system that monitors network or host activity and looks for signs of suspicious or malicious behavior. Network‑based IDS (NIDS) sit on the network and inspect packets as they flow, while host‑based IDS (HIDS) focus on logs, files, and processes on individual machines. Traditional IDS techniques often rely on signatures—known patterns of attacks—or simple rules. Newer approaches use anomaly detection and machine learning to spot behaviors that deviate from “normal,” even if the attack is previously unseen.\[[sciencedirect](https://www.sciencedirect.com/topics/computer-science/network-intrusion-detection)\]

This is where AI becomes a natural partner. Instead of hand‑crafting thousands of rules, ML‑based IDS learn statistical patterns of normal vs malicious traffic directly from data. Datasets like Edge‑IIoTset provide labeled examples of both benign and attack traffic, allowing models to be trained, validated, and compared under realistic industrial conditions. In my work, I used this to benchmark a range of models—from lightweight networks to complex spatio‑temporal GNNs—under federated learning, asking: *which ones actually work best when deployed at the edge on constrained devices?*\[[slogix](https://slogix.in/internet-of-things/edge-iiotset-a-new-comprehensive-realistic-cyber-security-dataset-of-iot-and-iiot-applications-for-centralized-and-federated-learning/)\]

I like to think of IDS as the nervous system of a digital infrastructure. Firewalls and access controls are like skin and bones—they define boundaries. IDS is the part that senses when something is wrong, sometimes before visible damage occurs. As our grids, factories, and cities become more connected, these gatekeepers are becoming smarter, more autonomous, and—thanks to AI—better at catching subtle threats that old rule‑based systems would miss.\[[fortinet](https://www.fortinet.com/resources/cyberglossary/intrusion-detection-system)\]

---

## **17\. LoRA in Federated Learning: Can Parameter-Efficient Fine-Tuning Save Edge Devices?**

Deep learning models are getting bigger, but edge devices are not magically turning into GPUs. That tension is what makes **LoRA (Low‑Rank Adaptation)** so interesting—especially when combined with federated learning.\[[arxiv](https://arxiv.org/abs/2504.16515)\]

LoRA’s core idea is simple: instead of fine‑tuning all the weights of a large model, you insert small low‑rank matrices (adapters) into certain layers and train only those. The original weights stay frozen, and the number of trainable parameters drops dramatically, which reduces memory, computation, and sometimes communication costs. In centralized setups, LoRA has already become a popular way to adapt large language or vision models with limited resources.\[[diva-portal](https://www.diva-portal.org/smash/get/diva2:1988818/FULLTEXT01.pdf)\]

Federated learning adds another twist: multiple clients (like edge devices or local controllers) collaboratively fine‑tune a global model by sending updates to a server without sharing raw data. Recent work on **FedLoRA** and related frameworks shows that we can exchange only the tiny LoRA modules between server and clients, instead of full model weights, making the entire process much more communication‑ and resource‑efficient. For edge environments, that’s crucial—these devices often have limited bandwidth, memory, and energy.\[[ieeexplore.ieee](https://ieeexplore.ieee.org/document/10901572/)\]

In my own research, I investigated how different model families behave in federated IoT intrusion detection under tight edge constraints, using Edge‑IIoTset as the benchmark. Even without LoRA, it was clear that heavyweight models are difficult to deploy at scale on resource‑constrained nodes. LoRA‑style parameter‑efficient fine‑tuning is a promising next step: you could imagine shipping a reasonably capable base model to all devices, then having each site fine‑tune only small adapters on its own data and share those back to the server. The big open question—and a great direction for future work—is how far we can push this idea in truly harsh environments like industrial IoT and smart grids without sacrificing robustness and security.\[[sciencedirect](https://www.sciencedirect.com/science/article/abs/pii/S1389128625008965)\]

---

## **18\. More Complex ≠ Better: The Surprising Truth About Graph Neural Networks for IoT Security**

When I started my thesis, I was very excited about Graph Neural Networks. They felt like the “fancy” option: they model relationships\! They capture structure\! Surely they must outperform simpler models on complex IoT intrusion detection tasks, especially if we combine temporal and spatial information in spatio‑temporal GNNs. Reality, as usual, was more nuanced.

In my work, I built a unified federated benchmarking framework and compared a spectrum of models—from MLPs and CNN‑style architectures to several spatio‑temporal GNN variants—on the Edge‑IIoTset dataset under realistic edge constraints. The GNNs were more computationally heavy and communication‑demanding in the federated setting, which already made them less attractive for low‑power devices. The surprising part was that, on this particular dataset—with tabular traffic features and no explicit physical graph structure—GNN‑based models did not consistently outperform simpler baselines.\[[sciencedirect](https://www.sciencedirect.com/science/article/pii/S2667305323001230)\]

This doesn’t mean GNNs are “bad” for security. It means that **model complexity has to be justified by the structure of the data and the deployment constraints.** Edge‑IIoTset represents network flows and device behavior, but not as an explicit graph of physical or logical connections. In that setting, the extra representational capacity of spatio‑temporal GNNs did not always translate into real‑world gains, especially when we factored in latency, memory, and federated communication overhead.\[[ieeexplore.ieee](https://ieeexplore.ieee.org/document/9751703/)\]

For me, the main lesson was philosophical as much as technical: more complex ≠ automatically better. Sometimes, a well‑tuned “simple” model, deployed in the right way, can be more practical, robust, and ethical—because it actually fits within the energy, hardware, and operational constraints of the system you’re trying to protect. In the future, I still want to explore GNNs on truly graph‑structured security data—like power grid topologies or industrial control graphs—but I’ll go into it with a more skeptical, data‑driven mindset instead of assuming that sophistication guarantees superiority.

**Phase 6 :**

## 19\. Occam's Razor in Machine Learning: Why the Simplest Model Often Wins

I used to think “real” machine learning meant deep, complex models with impressive diagrams and long names. If a model was simple—like logistic regression or a small MLP—it almost felt embarrassing to put it in a paper. Then I spent months benchmarking models on Edge‑IIoTset and met an old idea with a sharp edge: Occam’s razor.

Occam’s razor comes from philosophy: if two explanations fit the facts equally well, prefer the simpler one. In machine learning, we restate it as: among models that perform similarly on unseen data, we should usually choose the simpler model. Simple models tend to generalize better, are easier to interpret, and are less likely to overfit noisy training data—especially when your dataset is messy, imbalanced, or shifting over time.

In my thesis, I compared complex spatio‑temporal GNNs with much simpler architectures for federated IoT intrusion detection. I expected the GNNs to clearly dominate, but on the Edge‑IIoTset dataset—with mostly tabular traffic features and no explicit graph topology—this wasn’t always true. Sometimes, a well‑tuned “boring” model delivered similar performance with a fraction of the computational cost, memory footprint, and training instability under federated conditions.

Occam’s razor doesn’t say “always use the simplest model.” It says: when performance is comparable, stop worshipping complexity for its own sake. Now, whenever I’m tempted to propose a fancy architecture, I ask three questions:

1. Does the data really have rich structure that simpler models can’t capture?  
2. Do we have enough high‑quality data to justify the complexity?  
3. Can the target hardware—edge devices, microcontrollers, or smart grid controllers—actually run this reliably?

If the answer is “not really,” I don’t feel bad about choosing the simpler model anymore. In fact, it feels like a small act of intellectual honesty.

## 20\. How I Submitted My First Q1 Journal Paper: A Step-by-Step Guide for New Researchers

Submitting my first Q1 journal paper felt like standing in front of a very tall door with a tiny key. I remember staring at the “Submit Manuscript” button for almost an hour, half convinced some popup would say, “Sorry, this journal is not for people like you.” But I clicked it. And that click was the end of one journey and the beginning of another.

Most people only see the final outcome—“accepted” or “rejected”—but the process has its own rhythm. For a typical reputable journal, your paper goes through internal checks, then editor screening, then external peer review, then one or more rounds of revision before final acceptance. Q1 and Q2 journals screen heavily at the beginning: they look for scope fit, clear contribution, and a professional structure before they even think about sending it to reviewers. That means your title, abstract, and first few pages carry more weight than you think.

Behind my paper, though, there was never just “me.” From the very beginning, my advisor, Dr. Attaphongse, was quietly shaping the work into something Q1‑worthy. He didn’t just correct sentences; he gave direction. When I felt lost between too many ideas, he helped me find a clear research question. When my drafts were messy, he showed me how to structure the story so that the contribution was visible and honest. Every major decision—dataset choice, experimental design, framing of contributions—was stronger because he took the time to challenge me, guide me, and trust me with real responsibility.

Here’s how we approached my first Q1 submission, step by step:

1. Choosing the journal.  
   With his guidance, I didn’t just chase the highest quartile; we looked at scope, recent papers, and how well my work fit the conversation in that journal. He encouraged me to aim high but also to be realistic about where federated learning and IoT security would be genuinely appreciated.  
2. Clarifying the contribution.  
   My advisor pushed me to answer two brutal questions in the introduction: “What exactly is new?” and “Why should anyone care?” We framed the paper around a unified federated benchmarking framework and a careful empirical study of model complexity vs edge constraints, not just yet another model. On days when I doubted whether my work was “enough,” his belief in the contribution gave me the courage to keep polishing instead of giving up.  
3. Structuring the paper.  
   Together, we refined a simple mental template:  
   * Introduction: gap \+ why it matters  
   * Related work: what others tried and where they fall short  
   * Methodology: what we built and how  
   * Experiments: what we measured and why these metrics  
   * Discussion: what surprised us, what didn’t, and what it means  
   * Conclusion: what changes because of this work  
     His comments on my drafts were detailed and sometimes tough, but always fair. Each round made the paper sharper.  
4. Pre‑review polishing.  
   Before submission, he treated the manuscript like something that carried both our names and AIT’s name. He highlighted small formatting issues I didn’t even see, pushed me to fix reference details and figure captions, and reminded me that reviewers notice these things. It was in these final, quiet edits that I realized how much he cared—not just about publication, but about me learning to do things properly.

Then came the waiting. Credible journals usually take weeks to a few months for a first decision; anything “peer‑reviewed and accepted” in a few days is a serious red flag. During that time, when my anxiety spiked (“What if it’s a desk rejection?”), it was again my advisor who gave me perspective: this is normal, this is how science works, patience is part of the process. When reviews finally arrive—whatever they say—I know he will stand beside me for the revisions, just as he did during the drafting.

I am deeply aware that my first Q1 submission is not just a personal achievement; it is the result of someone believing in me early, giving me chances, and investing time he could have spent on his own work. Dr. Attaphongse didn’t just help with the paper—he helped me grow into someone who *could* write that paper at all. His guidance has shaped my research habits, my standards, and even how I see myself. I don’t think of his name on the paper as a formality; to me, it is a constant reminder that I didn’t walk this path alone.

For anyone preparing their first Q1 submission, here’s what I wish I had known earlier:

* Rejection is normal; desk rejections are not a verdict on your worth.  
* Your story (gap, contribution, impact) matters as much as your equations.  
* A good advisor is not just an academic supervisor—they can become a source of strength and a positive force in your life far beyond a single paper.

When I finally saw the paper ready to submit, I didn’t feel like I had “arrived.” I felt grateful—that I had an advisor who trusted me enough to treat this as my work, corrected me when I needed it, and quietly opened a door I might never have reached on my own.

None of this chapter of my journey would exist without the guidance of my advisor, Dr. Attaphongse, whose patience, direction, and belief in me turned a fragile idea into a Q1‑ready paper and a stronger version of myself.

## 21\. Responsible AI: Why Guardrails Matter When Machines Make Decisions About Critical Infrastructure

It’s one thing for an AI model to recommend a song or a movie. It’s very different when AI helps control a power grid, a microgrid, or an industrial plant. In critical infrastructure, AI mistakes don’t just mean “oops, wrong recommendation”—they can lead to blackouts, equipment damage, or safety incidents. That’s why responsible AI in this context is not a buzzword; it’s a safety requirement.

Governments and infrastructure agencies are increasingly explicit about this. Guidance for AI in critical infrastructure emphasizes human oversight, strong cybersecurity, careful data handling, and continuous monitoring. Systems should be designed with “security by design” and “defense in depth” in mind, not treated as isolated ML demos dropped into a sensitive environment. New challenges like the “AI for Grid Resilience and Security” competitions explicitly mention guardrails around mission alignment, security, operational realism, and trust and transparency of AI outputs.

My own research on federated intrusion detection and edge intelligence sits close to this world. If we deploy IDS models at the edge of a smart grid or industrial network, we’re implicitly trusting them to flag attacks and anomalies reliably. That raises several hard questions:

* What happens if the model is wrong—and who is accountable?  
* How do we prevent data used to train the model from leaking sensitive operational details?  
* How do we detect if someone is attacking the AI system itself, not just the underlying network?

For me, “responsible AI” in critical infrastructure means at least four things:

1. Humans stay in the loop.  
   AI should support human operators, not silently override them. Critical decisions should always have human oversight.  
2. Clear boundaries and guardrails.  
   We need explicit limits on where AI can and cannot act autonomously, what data it can access, and how its outputs are used.  
3. Robustness and security from day one.  
   Treat the AI system itself as part of the attack surface. That means hardening the training pipeline, monitoring inputs and outputs, and logging behavior for incident response.  
4. Transparency and documentation.  
   Even if a model is complex, operators should understand its basic behavior, assumptions, and limitations. Hidden, “mysterious” models are risky in environments where lives and infrastructure are at stake.

As I move toward potential PhD work on smart grids, federated learning, and energy systems, this idea of guardrails is becoming central in how I think. Building accurate models is only the first step. Building trustworthy, accountable, and well‑bounded models is the real challenge—especially when the lights in someone’s home might depend on them.

**Phase 7 :**

## **22\. Agentic AI Workflows: What Happens When AI Systems Start Making Decisions Autonomously?**

Most of us met AI in its “polite assistant” phase: you ask a question, it answers, and that’s the end of the story. **Agentic AI** is different. Instead of waiting for every instruction, these systems can take a high‑level goal—“summarize these documents and draft an email,” “monitor this grid and suggest actions,” “run this weekly report”—and then **plan, act, and adjust** across multiple steps with minimal human supervision.\[[arxiv](https://arxiv.org/html/2512.08769v1)\]

In an **agentic workflow**, an AI agent doesn’t just generate text. It breaks a goal into sub‑tasks, decides which tools or APIs to call, executes those calls, reads the results, and loops until some success condition is met. Think of it as moving from a Q\&A chatbot to a junior colleague who can:\[[meta-intelligence](https://www.meta-intelligence.tech/en/insight-agentic-workflow)\]

* interpret your objective,  
* design a mini‑project plan,  
* call other services (databases, search, simulations), and  
* come back with a finished result, not just an answer.\[[appen](https://www.appen.com/blog/ai-agentic-workflow)\]

Under the hood, many agentic systems share similar building blocks:

* **Perception** – understanding the user’s request and environment.\[[meta-intelligence](https://www.meta-intelligence.tech/en/insight-agentic-workflow)\]  
* **Planning** – decomposing complex goals into a task graph or sequence.\[[appen](https://www.appen.com/blog/ai-agentic-workflow)\]  
* **Tool use** – deciding when to call APIs, databases, or other agents.\[[orkes](https://orkes.io/blog/agentic-ai-explained-agents-vs-workflows/)\]  
* **Memory** – keeping track of what’s been done so far and what’s still pending.\[[digitalocean](https://www.digitalocean.com/community/conceptual-articles/build-autonomous-systems-agentic-ai)\]  
* **Guardrails** – constraints, safety checks, and human‑in‑the‑loop controls so the agent doesn’t go “off script.”\[[linkedin](https://www.linkedin.com/posts/rohit-ghumare_agenticai-aiworkflows-aiagents-activity-7349761667573985280-MfBP)\]

What makes this exciting for someone like me—who cares about federated learning, IoT, and smart grids—is that agentic AI is naturally suited for **complex, data‑rich environments**. Imagine a future system that can: watch sensor streams, call intrusion detection models, consult power forecasts, and propose safe control actions, all while respecting strict safety and privacy rules. We’re not fully there yet, and guardrails are critical, but agentic workflows are a glimpse of where “AI as tools” might evolve into “AI as coordinated teammates” in critical infrastructure.\[[lucinity](https://lucinity.com/blog/understanding-agentic-ai-the-future-of-autonomous-workflows)\]

---

## **23\. Deep Reinforcement Learning Explained: Teaching Machines to Make Smarter Decisions Over Time**

If supervised learning is like grading homework with an answer key, **reinforcement learning (RL)** is more like raising a child or training a dog. You don’t give the agent the correct action for every situation; you let it act, then **reward or punish** it based on what happens, and over time it learns which behaviors work best. When we add deep neural networks to this—letting them process rich inputs like images, sensor readings, or complex states—we get **Deep Reinforcement Learning (DRL)**.\[[huggingface](https://huggingface.co/learn/deep-rl-course/en/unit4/what-are-policy-based-methods)\]

In RL, everything revolves around four key pieces:\[[sciencedirect](https://www.sciencedirect.com/topics/computer-science/deep-reinforcement-learning)\]

* An **environment** (a game, a robot, a traffic system, an energy grid).  
* An **agent** that chooses actions.  
* A **state** describing the current situation.  
* A **reward** signal that says how good or bad each outcome is.

The agent’s goal is to learn a **policy**—a mapping from states to actions—that maximizes its long‑term reward, not just immediate gain. DRL uses deep networks as function approximators so the agent can handle huge, complicated state spaces: think of an Atari game screen, robot camera images, or high‑dimensional sensor data. Algorithms like DQN, PPO, and actor–critic methods differ in how they estimate value functions and update policies, but they all share this trial‑and‑error learning loop.\[[youtube](https://www.youtube.com/watch?v=1Y_zbDa8u3E)\]\[[spinningup.openai](https://spinningup.openai.com/en/latest/spinningup/rl_intro.html)\]

What makes DRL exciting is its ability to discover strategies we didn’t explicitly program. It has already been used for game‑playing, robotics, recommendation systems, and complex control tasks. For future work in smart grids and IoT, DRL hints at agents that could, for example, learn **when** to charge or discharge batteries, **how** to route power in microgrids, or **when** to trigger defensive actions in a cyber‑physical system—always balancing short‑term rewards (like cost) with long‑term stability and safety. The challenge, as always, is to combine this learning power with strong constraints and guardrails, especially when we let these systems influence real‑world infrastructure.\[[geeksforgeeks](https://www.geeksforgeeks.org/blogs/applications-of-reinforcement-learning-in-real-world/)\]

---

If you want, I can next:

* Make these a bit more personal (e.g., “how I first tried RL in code” or “how agentic AI feels from a researcher’s perspective”), or  
* Help you connect Phase 7 explicitly to your future smart‑grid PhD interests so the blog reads like one continuous journey.

**Phase 8** 

## **Smart grids 101**

***24\. Smart Grids 101: How AI is Transforming the Way We Manage Electricity***

When people hear “smart grid”, they often imagine something abstract and futuristic. In reality, smart grids are just power systems that finally started using sensing, communication, and AI as first‑class citizens instead of afterthoughts. Traditional grids were built for one‑way power flow from large generators to passive consumers; smart grids add two‑way information and control so the system can react in real time to changing demand, renewables, and faults.

At a technical level, a smart grid layers communication networks on top of physical infrastructure: smart meters at homes, sensors in substations, phasor measurement units, and intelligent electronic devices all generate continuous data streams. Protocols like IEC 61850 enable standardized communication for protection and control, making it possible to coordinate relays, breakers, and substations at millisecond scales instead of relying only on slow human interventions. This is exactly the world that researchers like Dr Narottam Das work in: power and energy systems, smart grid systems, and power system communications.

AI becomes essential once you have this much data. Forecasting models predict demand at different time scales; reinforcement learning agents can tune voltage and reactive power; anomaly detection models spot unusual patterns that might indicate equipment faults or cyber‑attacks. In parallel, optimization algorithms orchestrate distributed energy resources like rooftop solar, batteries, and electric vehicles so that the grid stays stable even as generation becomes more intermittent. Many of the student projects Dr Das supervises—such as domestic energy management, microgrid control, and predictive maintenance in photovoltaic systems—sit precisely at this intersection of data, control, and energy.

For me, coming from IoT intrusion detection and federated learning, smart grids feel like a natural next step. A “smart grid” is essentially a massive, safety‑critical IoT network where each node is both a data source and an actuator. The same questions we ask in networking and security—Who can access this data? How do we detect anomalies? Where should models run?—reappear, but now with the added constraint that mistakes can bring down power to an entire community. That makes it an exciting and responsible domain for future research.

---

## Federated learning for grids

*25\. Federated Learning for Smart Grids: Why Decentralized AI Makes Perfect Sense for Energy Networks*

Smart grids generate huge volumes of sensitive data: household smart meter readings, inverter logs, substation measurements, and microgrid control signals. Centralizing all of this data in the cloud is often impractical (because of bandwidth and latency) and sometimes undesirable (because of privacy and regulatory concerns). That is exactly the scenario federated learning was designed for—training models collaboratively without shipping raw data off the devices or substations where it is generated.

In federated learning, each client (for example, a substation controller, a building energy management system, or even a cluster of smart meters) trains a local model on its own data and sends only model updates to a coordinating server. The server aggregates these updates into a global model and redistributes it, iterating until convergence. My master’s work used this paradigm for IoT intrusion detection, benchmarking a spectrum of models—from simple MLPs to complex spatio‑temporal GNNs—across constrained edge devices. The same design pattern could be repurposed for smart grid tasks like localized load forecasting, anomaly detection in feeders, or predictive maintenance for transformers.\[[techrxiv](https://www.techrxiv.org/doi/10.36227/techrxiv.18857336)\]

The benefits line up nicely with what power engineers care about. Privacy is improved because raw consumption profiles never leave the premises; only compressed model updates are shared. Communications are lighter because gradients are much smaller than entire datasets, which is important when the communication network itself is part of the critical infrastructure. Models can also adapt to local conditions—urban vs rural feeders, different PV penetration levels—while still benefiting from global knowledge. For a supervisor working on microgrids, PV systems, and transformer health monitoring, federated learning offers a way to bring modern AI into their domain without violating practical and regulatory constraints.

Of course, federated learning is not a silver bullet. Smart grid data can be highly non‑IID: consumption patterns differ drastically between regions, seasons, and customer types, and communication links can be unreliable. My previous work on federated STGNNs already showed that more complex models are not always better under such constraints. This opens an interesting research space: can we design lightweight, robust federated models specifically tailored to smart grid topologies and variability?

---

## Privacy in smart energy

*26\. The Privacy Problem in Smart Energy: Why We Can’t Just Send Everyone’s Power Data to the Cloud*

Smart meters and connected energy devices are amazing for grid operators: they provide fine‑grained visibility into demand, enable dynamic tariffs, and support sophisticated control strategies. But the same high‑resolution data can reveal surprisingly intimate details about people’s lives—when they are home, when they sleep, which appliances they use, and even patterns that correlate with health or income. That’s the core privacy problem in smart energy systems.

Research on domestic energy management, such as projects analyzing household load profiles and control strategies, implicitly touches this issue: any algorithm that optimizes energy usage has access to behavior patterns that users might not want to share broadly. If all raw time‑series data is pushed to a hyperscale cloud, we increase the attack surface and make it easier for adversaries—or even legitimate third parties—to profile consumers at scale. For critical infrastructure like smart grids, that risk is not just personal; it also has national security implications when aggregated.

This is where decentralization and privacy‑preserving machine learning become more than buzzwords. Techniques like federated learning keep data local while still enabling global model training, and differential privacy can add noise to updates to make it harder to reconstruct specific individual behaviors. Edge analytics can perform tasks such as anomaly detection or basic forecasting on in‑home gateways or substation controllers, so only aggregated insights flow upward. From a PhD perspective, aligning with supervisors who work on microgrids, energy management, and PV systems means you can propose solutions that are technically grounded in real hardware and power systems, not just in abstract ML theory.

To me, the interesting question is not “Should we use smart meters?” but “How can we design smart energy systems that are *privacy‑by‑design*?” That includes technical tools (federated learning, secure aggregation, encryption) and policy questions (data retention periods, consent, and who controls access). My background in IoT security and federated models gives me a starting point; the smart grid domain adds very real stakes and constraints.

---

## Anomaly detection in solar

*27\. Anomaly Detection in Solar Panels: How Machine Learning Spots Faults Before They Become Failures*

Solar panels look static from the outside, but electrically they live dynamic lives: shading, soiling, degradation, and wiring issues can all change their behavior over time. If we wait until a panel “dies” or output drops dramatically, we lose energy, money, and sometimes damage associated equipment. That is why anomaly detection and predictive maintenance for PV systems has become a vibrant research area, including projects supervised by researchers like Dr Das on “Proactive Fault Detection using Machine Learning to Aid Predictive Maintenance in Photovoltaic Systems.”

The basic idea is simple: learn what “normal” looks like, then flag deviations early. ML models can be trained on historical voltage, current, irradiance, and temperature data from PV arrays to capture typical operating patterns under different conditions. Once deployed, they continuously compare live measurements to the learned patterns and raise alerts when something looks off—partial shading, connector failures, inverter issues, or emerging degradation. Some approaches use traditional time‑series models, others employ neural networks or even graph‑based models to capture spatial relationships between panels or strings.

There is a natural bridge here to my own work on IoT intrusion detection. In both cases, we are trying to spot subtle anomalies in high‑volume sensor streams before they escalate into incidents—whether that incident is a cyberattack on an IoT device or a costly failure in a solar farm. The Edge‑IIoTset dataset I worked with, for example, captured multi‑modal IoT traffic under benign and malicious scenarios, and our models learned to distinguish normal from abnormal patterns at the edge. A future PhD could apply similar ideas to PV arrays and microgrids: edge devices running lightweight anomaly detectors that protect both cyber and physical assets.\[[techrxiv](https://www.techrxiv.org/doi/10.36227/techrxiv.18857336)\]

For someone like me, who cares about both security and sustainability, PV anomaly detection is more than an optimization problem. Every “saved” panel or avoided failure means more clean energy delivered over the system’s lifetime. Combining energy engineering expertise from a supervisor with my background in federated and graph‑based models could lead to fault detection systems that are not only accurate, but also privacy‑preserving and deployable on resource‑constrained hardware in the field.

---

## Sustainable AI and energy

*28\. Sustainable AI: The Carbon Cost of Training Machine Learning Models (And What We Can Do About It)*

The irony of AI for sustainability is that training large models can itself consume a lot of energy. As models grow in parameter count and training datasets scale up, so does the electricity required to train and run them. That raises a hard question: how do we ensure our AI work *helps* decarbonize the world more than it contributes to emissions? Competitions like the Low‑Power Computer Vision Challenge (LPCVC) explicitly push researchers to think about energy efficiency, rewarding solutions that run accurately under tight power budgets.\[[qualcomm](https://www.qualcomm.com/developer/blog/2025/05/low-power-computer-vision-challenge-with-qualcomm-ai-hub)\]

More recently, OpenAI’s “Parameter Golf” challenge asked participants to minimize loss on a fixed dataset under strict limits on model size (16 MB artifacts) and training time, forcing them to search for architectures and training tricks that deliver maximum performance per parameter and per joule. These community efforts are a reminder that scientific prestige doesn’t *have* to be tied only to model size; efficiency and elegance can be metrics too. My own participation in such challenges fits naturally with my research on edge‑friendly models for IoT intrusion detection, where the goal is always to do more with less—less compute, less memory, less bandwidth.\[[startuphub](https://www.startuphub.ai/ai-news/artificial-intelligence/2026/openai-s-parameter-golf-reveals-ai-s-role)\]

This connects directly to potential supervisors in power and renewable energy. Dr Das’s work on photovoltaic power systems, high‑efficiency solar cells, and microgrids is fundamentally about getting more useful work from each watt of energy. If we deploy AI to manage grids, optimize PV output, or detect faults, but the AI itself is bloated and wasteful, we’re missing the point. A “sustainable AI” agenda in this context could include: designing compact models suitable for edge controllers, co‑optimizing algorithms and hardware, powering computation with on‑site renewables, and using federated learning to avoid unnecessary data movement.

For me, sustainable AI is not just about guilt over GPU hours; it is about aligning the *entire* pipeline—from data collection and training to deployment and maintenance—with the physical realities of energy systems. Working at the intersection of federated learning, smart grids, and renewable energy would let me contribute models that are not only accurate and secure, but also respectful of the carbon and energy budget they operate within.

## **Final Ordered List of Posts (All Phases)**

## **Phase 1 — Early Academic Foundations (Bachelor’s / Medical AI)**

1. **Why Your Phone Could One Day Detect Skin Cancer Before Your Doctor Does**  
2. **\[Your second bachelor‑thesis‑related title from the earlier plan – keep the one you liked there\]**

## **Phase 2 — Industry Experience (QA Engineer)**

3. **From QA Engineer to AI Researcher: How Testing Shaped My Thinking About Model Reliability**  
4. **The Most Dangerous Bugs Aren’t Crashes: What Manual Testing Taught Me About Software Quality**  
5. **What Being the First QA Engineer on a Product Team Taught Me About Ownership**  
6. **Why Real Users Never Use Software the Way Developers Expect**  
7. **Can We Test AI the Way We Test Software? Lessons from My QA Background**

## **Phase 3 — Transition to Master’s & Research Mindset**

8. **\[Post about deciding to return to grad school / AIT journey – from earlier plan\]**  
9. **\[Post about choosing federated learning and IoT security as your research direction\]**  
10. **\[Post about first experiments / learning to read research papers\]**  
11. **\[Bridging QA mindset with research: how debugging experiments feels like debugging software\]**

***(Again, keep these aligned with the Phase 3 titles we already drafted in your earlier plan.)***

## **Phase 4 — Learning the Foundations**

12. **What is Federated Learning and Why It’s the Future of Privacy‑Preserving AI**  
13. **Graph Neural Networks 101: When Network Structure Actually Matters (And When It Doesn’t)**  
14. **Edge Computing and AI: Why the Future of Intelligence is Local, Not in the Cloud**

## **Phase 5 — Master’s Thesis Research**

15. **What is the Edge‑IIoTset Dataset and Why It Matters for Industrial Security Research**  
16. **Intrusion Detection Systems: The AI Gatekeepers Defending Our Connected World**  
17. **LoRA in Federated Learning: Can Parameter‑Efficient Fine‑Tuning Save Edge Devices?**  
18. **More Complex ≠ Better: The Surprising Truth About Graph Neural Networks for IoT Security**

## **Phase 6 — Becoming a Researcher**

19. **Occam’s Razor in Machine Learning: Why the Simplest Model Often Wins**  
20. **How I Submitted My First Q1 Journal Paper: A Step‑by‑Step Guide for New Researchers**  
21. **Responsible AI: Why Guardrails Matter When Machines Make Decisions About Critical Infrastructure**

## **Phase 7 — Exploring New Research Frontiers**

22. **Agentic AI Workflows: What Happens When AI Systems Start Making Decisions Autonomously?**  
23. **Deep Reinforcement Learning Explained: Teaching Machines to Make Smarter Decisions Over Time**

## **Phase 8 — Moving Toward Future PhD Interests**

24. **Smart Grids 101: How AI is Transforming the Way We Manage Electricity**  
25. **Federated Learning for Smart Grids: Why Decentralized AI Makes Perfect Sense for Energy Networks**  
26. **The Privacy Problem in Smart Energy: Why We Can’t Just Send Everyone’s Power Data to the Cloud**  
27. **Anomaly Detection in Solar Panels: How Machine Learning Spots Faults Before They Become Failures**  
28. **Sustainable AI: The Carbon Cost of Training Machine Learning Models (And What We Can Do About It)**

Pipa, the adorable bunny teacher with cream-colored fluffy fur, black oval eyes, rosy cheeks, a tiny pink nose, wearing a dusty pastel blue dress and a white daisy behind her left ear, stands beside one shiny red apple.

A large colorful number "1" floats beside the apple.

Pipa points at the apple and smiles.

Sparkles appear around the number.

Gentle bouncing animation.

Sunny meadow background with flowers and butterflies.

Camera slowly zooms in.

Ultra-cute preschool educational animation.

Use the uploaded image as the exact reference for Pipa.

Keep her face, expression, cream-colored fluffy fur, fluffy blond hair tuft, large upright ears with light pink inner ears, round black eyes, rosy cheeks, tiny pink nose, fine whiskers, white daisy behind her left ear, dusty pastel blue sleeveless dress, and overall proportions exactly the same. Do not redesign or alter the character.

Pipa, stands beside one shiny red apple.

A large colorful number "1" floats beside the apple.

Pipa points at the apple and smiles.

Sparkles appear around the number.

Gentle bouncing animation.

Sunny meadow background with flowers and butterflies.

Camera slowly zooms in.

High-quality stylized 3D animated cartoon with an original preschool aesthetic, bright pastel colors, soft rounded shapes, expressive facial animation, gentle cinematic lighting, smooth polished animation, and a joyful child-friendly atmosphere.

Keep the movement slow,gentle, and suitable for toddlers aged 2–5. Keep Pipa's appearance consistent with the uploaded reference image throughout the clip. 

