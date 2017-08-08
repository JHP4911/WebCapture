# Understanding the limits of deep learning

_Captured: 2017-04-03 at 17:10 from [venturebeat.com](https://venturebeat.com/2017/04/02/understanding-the-limits-of-deep-learning/)_

![](https://venturebeat.com/wp-content/uploads/2017/03/deeplearninglimits_VB_1200px_web.jpg?fit=930%2C698&strip=all)

[Artificial intelligence](https://venturebeat.com/2017/04/01/why-ai-needs-a-magic-moment/) has reached peak hype. News outlets report that companies have replaced workers with IBM Watson and algorithms are beating doctors at diagnoses. New AI startups pop up every day and claim to solve all your personal and business problems with machine learning.

Ordinary objects like juicers and Wi-Fi routers suddenly advertise themselves as "powered by AI". Not only can smart standing desks remember your height settings, they can also [order you lunch](https://www.autonomous.ai/).

Much of the AI hubbub is generated by reporters who've never trained a neural network and startups or those hoping to be acquihired for engineering talent despite not solving any real business problems. No wonder there are so many misconceptions about what AI can and cannot do.

## **Deep learning is undeniably mind-blowing**

Neural networks were invented in the 60s, but recent boosts in big data and computational power made them actually useful. A new discipline called "deep learning" arose and applied complex neural network architectures to model patterns in data more accurately than ever before.

The results are undeniably incredible. Computers can now [recognize objects in images and video](http://karpathy.github.io/2014/09/02/what-i-learned-from-competing-against-a-convnet-on-imagenet/) and [transcribe speech to text](https://blogs.microsoft.com/next/2016/10/18/historic-achievement-microsoft-researchers-reach-human-parity-conversational-speech-recognition/) better than humans can. Google [replaced](https://research.googleblog.com/2016/09/a-neural-network-for-machine.html) Google Translate's architecture with neural networks and now machine translation is also closing in on human performance.

The practical applications are mind-blowing as well. Computers can [predict crop yield](https://cs.stanford.edu/~ermon/group/website/papers/jiaxuan_AAAI17.pdf) better than the USDA and indeed [diagnose cancer](https://med.stanford.edu/news/all-news/2016/08/computers-trounce-pathologists-in-predicting-lung-cancer-severity.html) more accurately than elite physicians.

John Launchbury, a Director at DARPA, [describes](http://www.darpa.mil/attachments/AIFull.pdf) three waves of artificial intelligence: 1) Handcrafted knowledge, or expert systems like IBM's Deep Blue or Watson, 2) Statistical learning, which includes machine learning and deep learning, and 3) Contextual adaption, which involves constructing reliable, explanatory models for real world phenomena using sparse data, like humans do.

As part of the current second wave of AI, deep learning algorithms work well because of what Launchbury calls the "manifold hypothesis" (see below). In simplified terms, this refers to how different types of high-dimensional natural data tend to clump and be shaped differently when visualized in lower dimensions.

![Image Credit: John Launchbury / DARPA](http://venturebeat.com/wp-content/uploads/2017/03/darpa_manifolds_750px_web.jpg?resize=750%2C406&strip=all)

> _Above: Image Credit: John Launchbury / DARPA_

By mathematically manipulating and separating data clumps, deep neural networks can distinguish different data types. While neural nets can achieve nuanced classification and predication capabilities they are essentially what Launchbury [calls](https://www.youtube.com/watch?v=-O01G3tSYpU) "spreadsheets on steroids."

![Image Credit: John Launchbury / DARPA](http://venturebeat.com/wp-content/uploads/2017/03/darpa_manifolds_separation_750px_web.jpg?resize=750%2C405&strip=all)

> _Above: Image Credit: John Launchbury / DARPA_

## **Deep learning also has deep problems**

At the recent [AI By The Bay](https://ai.bythebay.io/) conference, Francois Chollet emphasized that deep learning is simply more powerful pattern recognition vs. previous statistical and machine learning methods. "The most important problem for A.I today is abstraction and reasoning," explains Chollet, an AI Researcher at Google and famed inventor of widely used deep learning library [Keras](https://keras.io). "Current supervised perception and reinforcement learning algorithms require lots of data, are terrible at planning, and are only doing straightforward pattern recognition."

By contrast, humans "learn from very few examples, can do very long-term planning, and are capable of forming abstract models of a situation and manipulate these models to achieve extreme generalization."

Even simple human behaviors are laborious to teach to a deep learning algorithm. Let's examine the task of not being hit by a car as you walk down the road. If you go the supervised learning route, you'd need huge data sets of car situations with clearly labeled actions to take, such as "stop" or "move". Then you'd need to train a neural network to learn the mapping between the situation and the appropriate action.

If you go the reinforcement learning route, where you give an algorithm a goal and let it independently determine the ideal actions to take, the computer would need to die thousands of times before learning to avoid cars in different situations.

"You cannot achieve general intelligence simply by scaling up today's deep learning techniques," warns Chollet.

Humans only need to be told once to avoid cars. We're equipped with the ability to generalize from just a few examples and are capable of imagining (i.e. modeling) the dire consequences of being run over. Without losing life or limb, most of us quickly learn to avoid being overrun by motor vehicles.

While neural networks achieve statistically impressive results across large sample sizes, they are "individually unreliable" and often make mistakes humans would never make, such as classify a toothbrush as a baseball bat.

![Image Credit: John Launchbury / DARPA](http://venturebeat.com/wp-content/uploads/2017/03/misclassification_darpa_web.jpg?resize=306%2C324&strip=all)

> _Above: Image Credit: John Launchbury / DARPA_

Your results are only as good as your data. Neural networks fed inaccurate or incomplete data will simply produce the wrong results. The outcomes can be both embarrassing and damaging. In two major PR debacles, Google Images incorrectly classified African Americans as gorillas, while Microsoft's Tay learned to spew racist, misogynistic hate speech after only hours training on Twitter.

Undesirable biases may even be implicit in our input data. Google's massive Word2Vec embeddings are built off of 3 million words from Google News. The data set makes associations such as "father is to doctor as mother is to nurse" which [reflect gender bias](https://www.technologyreview.com/s/602025/how-vector-space-mathematics-reveals-the-hidden-sexism-in-language/) in our language. Researchers such as Tolga Bolukbasi of Boston University have taken to human ratings on Mechanical Turk to perform "hard de-biasing" to undo the associations.

Such tactics are essential since, according to Bolukbasi, "word embeddings not only reflect stereotypes but can also amplify them." If the term "doctor" is more associated with men than women, then an algorithm might prioritize male job applicants over female job applicants for open physician positions.

Finally, Ian Goodfellow, inventor of generative adversarial networks (GANs), [showed](https://openai.com/blog/adversarial-example-research/) that neural networks can be deliberately tricked with adversarial examples. By mathematically manipulating an image in a way that is undetectable to the human eye, sophisticated attackers can trick neural networks into grossly misclassifying objects.

![Image Credit: Ian Goodfellow](http://venturebeat.com/wp-content/uploads/2017/03/ian_goodfellow_adversarial_attacks.png?resize=470%2C178&strip=all)

> _Above: Image Credit: Ian Goodfellow_

## **What's beyond deep learning? **

How can we overcome the limitations of deep learning and proceed towards general artificial intelligence? Chollet's initial plan of attack involves using "super-human pattern recognition like deep learning to augment explicit search and formal systems", starting with the field of mathematical proofs. Automated Theorem Provers (ATPs) typically use brute force search and quickly hit combinatorial explosions in practical use. In the [DeepMath](https://arxiv.org/abs/1606.04442) project, Chollet and his colleagues used deep learning to assist the proof search process, simulating a mathematician's intuitions about what lemmas might be relevant.

Another approach is to develop more explainable models. In handwriting recognition, neural nets currently need to be trained on tens to hundreds of thousands of examples to perform decent classification. Instead of looking at just pixels, however, Launchbury of DARPA explains that generative models can be taught the strokes behind any given character and use this physical construction information to disambiguate between similar numbers, such as a 9 or a 4.

Yann LeCun, inventor of convolutional neural networks (CNNs) and director of AI research at Facebook, proposes "[energy-based models](https://scholar.google.com/citations?view_op=view_citation&hl=en&user=WLN3QrAAAAAJ&cstart=20&pagesize=80&citation_for_view=WLN3QrAAAAAJ%3A8k81kl-MbHgC)" as a method of overcoming limits in deep learning. Typically, a neural network is trained to produce a single output, such as an image label or sentence translation. LeCun's energy-based models instead give an entire set of possible outputs, such as the many ways a sentence could be translated, along with scores for each configuration.

Geoffrey Hinton, widely called the "father of deep learning" wants to replace neurons in neural networks with "capsules" which he believes more accurately reflect the cortical structure in the human mind. "Evolution must have found an efficient way to adapt features that are early in a sensory pathway so that they are more helpful to features that are several stages later in the pathway," Hinton [explains](https://www.reddit.com/r/MachineLearning/comments/2lmo0l/ama_geoffrey_hinton/). He hopes that capsule-based neural network architectures will be more resistant to the adversarial attacks that Goodfellow illuminated above.

Perhaps all of these approaches to overcoming the limits of deep learning have truth value. Perhaps none of them do. Only time and continued investment in AI research will tell.

_Mariya Yao is the Head of Design and Engagement at Topbots.com, a media and marketing firm specializing in chatbots and conversational agents. _

_This article originally appeared on [Topbots](http://www.topbots.com/understanding-limits-deep-learning-artificial-intelligence/)._