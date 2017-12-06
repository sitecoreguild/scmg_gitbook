# What is Sitecore Commerce?

## Explanation Of This Section

Sitecore Commerce is the commerce offering from Sitecore. As someone new I got confused about the various components that are involved in the Sitecore + Commerce equation. There are a lot of terms kicking around, I tried to clear things up but even still I was confused. Thanks a lot to Timothy Stelemen for the information on the history and everyone else for your edits that have helped us clear things up.

If anyone else has alterations or additional information to add, please feel free to edit the document or any of the other sections made available. This is a community effort. Look forward to learning together.

I did find this article that actually says it better than I did. The [Oshyn blog titled Sitecore Commerce Overview and Installation](https://l.facebook.com/l.php?u=http%3A%2F%2Fwww.oshyn.com%2Fblogs%2Fsitecore-commerce-overview-and-installation%3Fpage%3DNaN&h=ATOwthe3pqiiiTHcMvOFNxSU-jJAKPR01wz_5DFZ0nvGbEjk85rs7_uag0wU5ZxIbCDrPqEyJ-KbqmwQj_s7HGLw4mty0spWdLeJ5ykiVJVZiswEFF4Iqls2vFo5IfzpUml3xmXmAoo) Thanks Prashanth Nittala for writing such a great article.

## Sitecore Commerce vs Sitecore Commerce powered by Dynamics AX

Commerce Server History by Timothy Steleman

Commerce Server has never been integrated with Dynamics AX, it has been a standalone, Microsoft owned, product since 1999 \(back then it was called Site Server - Commerce Edition. In 2002 it was one of the first products to be moved to .NET, and called commerce server 2002 \(unfortunately, not all code bits got ported over to .net and some COM+ bits remained, event to this day, well the last ones have now just been removed in the latest release by the Sitecore team\). In 2009/2010, after a failed market pitch to make Sharepoint the CMS of the future, and to integrate commerce server deeply into it, Microsoft sold Commerce Server - and the cactus commerce team that had always been responsible for it \(the Canada based folks\) - to Ascentium, now Smith, an agency that had historically done a good bit of work with Commerce Server. Now, meanwhile, Sitecore had an abstract commerce layer in the works called Commerce Connect and there were \(and still are\) a few 3rd party vendors that had an eCommerce product that integrated with it \(InSite, Znode back in the day, and Ascentium built an integration for Commerce Server too\). So when Sitecore wanted to add commerce capabilities to its platform, the looked for products and Commerce Server was a good fit because 1\) Ascentium had already built the Commerce Connect bits to integrate and 2\) Commerce Server still had a decent enterprise install base from its earlier life at Microsoft. Commerce Server came with some outdated business user applications \(windows desktop UIs like catalog manager, customer and orders managers etc, ...\) and that's what the Sitecore Commerce team has focused on improving initially \(the first of which was the merchandising manager application\). By now they have of course rewritten the whole order system and moved that to .net core and the other business user applications. By Sitecore v9, all the code bits of the old commerce server will be removed. \(read next comment for the dynamics AX story\)

Sitecore Commerce Powered by Dynamics AX Explained by Timothy Steleman

Alright, so Sitecore Commerce powered by Dynamics AX is a totally different story, one that has little, or better nothing, to do with commerce server at all. Remember I told you that Sitecore has it's Commerce Connect layer as an abstract integration layer for commerce functionality? Well, a few years ago, a large home decoration and furniture retailer wanted to implement eCommerce, but integrated with its Point of sale system, which happened to be Dynamics AX for retail. So Sitecore and Microsoft, along with the implementation partner \(one of the biggest ones, closely tied to Microsoft\) built the Commerce Connect integration for Dynamics AX for retail. Microsoft, wanting to push its Dynamics AX for retail products, and Sitecore wanting to push its platform then jointly pushed to 'productize' this connector that was built and this then became Sitecore Commerce powered by Dynamics AX. So it's not related to Commerce Server at all, it's just another implementation of the Commerce Connect integration API

## Commerce Connect

So the way I understand it is that the Commerce Connect as a general mechanism for Commerce applications like uCommerce \(with support for Umbraco, Kentico as well as Sitecore\) and InSite Commerce \(a B2B focused product\) to integrate with Sitecore. Companies like NishTech offer an InSite Connector that further accellerates working with InSite and Sitecore.

## How Do All The Commerce Related Components Fit Together

Well the best diagram I found so far is the one in the

[Oshyn blog titled Sitecore Commerce Overview and Installation](https://l.facebook.com/l.php?u=http%3A%2F%2Fwww.oshyn.com%2Fblogs%2Fsitecore-commerce-overview-and-installation%3Fpage%3DNaN&h=ATOwthe3pqiiiTHcMvOFNxSU-jJAKPR01wz_5DFZ0nvGbEjk85rs7_uag0wU5ZxIbCDrPqEyJ-KbqmwQj_s7HGLw4mty0spWdLeJ5ykiVJVZiswEFF4Iqls2vFo5IfzpUml3xmXmAoo)

Thanks Prashanth Nittala for writing such a great article.

If you are interested in how the Sitecore Commerce Powered By Dynamics AX works this article called A simple architectural overview of

[Sitecore Commerce powered by Microsoft Dynamics](https://l.facebook.com/l.php?u=https%3A%2F%2Fwebsterian.com%2F2016%2F10%2F20%2Fa-simple-architectural-overview-of-sitecore-commerce-powered-by-microsoft-dynamics%2F&h=ATOwthe3pqiiiTHcMvOFNxSU-jJAKPR01wz_5DFZ0nvGbEjk85rs7_uag0wU5ZxIbCDrPqEyJ-KbqmwQj_s7HGLw4mty0spWdLeJ5ykiVJVZiswEFF4Iqls2vFo5IfzpUml3xmXmAoo)

provides a good diagram.

