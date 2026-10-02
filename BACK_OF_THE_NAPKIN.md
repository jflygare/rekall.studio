# Rekall.studio

![For the memory of a lifetime](docs/inspiration/for-the-memory-of-a-lifetime.png)

> [!WARNING]
> rekall.studio is a personal project (Jesse Flygare) and POC intended to explore and demonstrate the capabilities of AI. It may use AI tools and services that do not provide robust protection of identity or misuse.

## Concept
rekall.studio is a homage to **[Rekall Industries](https://totalrecall.fandom.com/wiki/Rekall#Rekall)** from the classic 1990 film **[Total Recall](https://www.imdb.com/title/tt0100802/)**, reimagined as a website where users can create "memories" (images and videos) of themselves participating in ideal vacations or impossible adventures, as if they had actually lived them.

The site focuses on:
- Ease of use: Zero learning curve and no AI experience is needed to use the site.
- Authenticity: Generated content is not gimmicky or contrived. If it were not so fantastical, it could pass as genuine.
- Quality over customization: User creativity is allowed within the limits of the theme.

The web app makes heavy use of generative AI models, tools and services. Models are trained on user images/video and then used to generate new media without the need for further image references or anchoring. AI is used to aid in the training of new models by filtering out and cleaning up (when possible) user provided media. This includes extracting the best training images from videos based on feature clarity, gesture diversity and full body captures. LoRAs and other strategies are used to maintain consistency and style accross models. AI is used to aid in the creation of naritives/promts for media generation.

At a high level, the typical workflow is:
1. User registers and establishes their persona via live photo and speech sampling
1. User imports (via upload or link) images and/or videos of themselves for model training
1. User selects preferred notification method of training completion
1. AI extracts trainable images from video
1. AI filters images to include only those of the user
1. AI enhances low resolution, blurry and low lit images
1. AI crops/removes unwanted elements so that only images suitable for model training remain
1. A clean base model is trained with the catalog of processed images
1. User is notified that studio is ready to use
1. User picks from pre-packaged memories or describes a custom memory
1. AI validates custom requests against theme adherence and rejects or enhances/tunes it into a suitable prompt
1. AI generates images using user's trained model and selected memory prompts
1. AI generates videos using the generated images as references on a video capable model
1. User sees content associated with their chosen memory as it becomes available and a status of queued generations
1. User can delete generated content and elect to generate more for an existing memory
1. User can start a new memory workflow


## Website
### Landing page
https://rekall.studio landing page gives users a taste of what memories they have missed, or are missing out on, but can create using the site. The page uses elements from the [**Rekall Industries** commercial](https://www.youtube.com/watch?v=lFAp13bbOFQ) from the film.

>*Would you like to ski Antarctica...  but snowed under with work?  
Do you dream of a vacation at the bottom of the ocean... but you can't float the bill?  
Have you always wanted to climb the mountains of Mars... but now you're over the hill?  
Then come to recall.studio, where you can create the memory of your ideal vacation, cheaper, safer and better than the real thing.*

Users can login or register for free (no credit card or payment method required) from the landing page.

### App
https://app.rekall.studio provides a workspace where registered users can manage the training of their model(s), the creation of new memories and manage existing memories. Users can also manage thier identity (avatar and speech sampling), account profile, preferences/settings and billing. The style is inspired by the Total Recall movie, without being overly retro.

New users must first establish their persona before accessing training and memory features. The free tier limits features to (TBD). Paid tiers unlock more features, including images, then videos, then custom memories.