# ✏ Managing content

## Landing page cards

The cards at the bottom of [the landing page](https://www.p2pu.org/en/) can be managed using the [NetlifyCMS interface](https://www-staging.p2pu.org/en/admin/#/collections/data/entries/landing%20page). The "cards" and "testimonials" lists are combined and sorted according to the order attribute in reverse order, so that when adding a new item to either list, the order must be manually set to a number higher than the highest number in either list to appear first.

Images can either be uploaded using the image widget, or set to an image URL hosted somewhere else like the P2PU Wordpress blog. When adding images, ensure that the image file size is appropriate (preferable much smaller than 200kb, but definitely not any larger!) since the landing page is the most viewed page.&#x20;

## Topic guides

Add topic guides using the [NetlifyCMS interface](https://www-staging.p2pu.org/en/admin/#/collections/topics). Click on add topic and fill in all fields exept the optional excerpt.

To make sure the image chosen works in the different display contexts, use the template on Figma.

To associate courses with the topic guide, a topic needs to be set for each course corresponding to an item in "search topics". For example, for "Job readiness" the topic is "job skills" and searching using that topic on the learning resources page will show you all the courses associated with the topic: [https://www.p2pu.org/en/learning-resources/?topics=job%20skills](https://www.p2pu.org/en/learning-resources/?topics=job%20skills)

Iow,&#x20;

* pick a topic, eg. 'language-learning'.&#x20;
* Add it in the "Search topics" field for the topic using the netlify interface ([https://www-staging.p2pu.org/en/admin/#/collections/topics/entries/language-learning](https://www-staging.p2pu.org/en/admin/#/collections/topics/entries/language-learning)).&#x20;
* Then use the django admin interface ([https://staging-learningcircles.p2pu.org/en/admin/studygroups/course/](https://staging-learningcircles.p2pu.org/en/admin/studygroups/course/)) to find the courses you wish to add, and make sure the topics are set in the "Topics" field as part of a comma separated list
