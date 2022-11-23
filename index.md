---
layout: default
---

1. Add a dedicated Piwik PRO element that will act as a container for the video. We can provide you with a template that will contain both HTML and CSS code.
2. The **Open Consent Form** button will trigger the Piwik PRO consent form to pop up, whether the consent has been already given or not.
3. Add a Custom content tag in Piwik PRO Tag Manager. The **Tag code** should contain an iframe element with the video.
4. In the tag settings, the **Element ID** should be the same as the id attribute (`id=""`) of the container Piwik PRO element (in this case `pp_embed_container`).
5. Choose the **consent type** that suits your case (we will use _Analytics_ for this PoC)
6. Create a **Page view trigger** and select the **Loaded all page elements (page load)** option.
7. Save the trigger and then save the tag.
8. You can now test the solution. The _Please give consent in order to see the content_ banner should be displayed as long as the visitor doesn't accept the _Analytics_ consent.
9. In case the user revokes the _Analytics_ consent the banner will be visible again after a page refresh.
