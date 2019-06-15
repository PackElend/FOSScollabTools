# FOSScollabTools
<details> 
  <summary><h2>Q1: The reason doing this</h2></summary>
Hello, our organization faces the same challenge since we hit the limits of the
free plan of slack and others, so this discussion was an inducement for doing
some research for the right alternative.  As there aren't little (luckily)
options around I may ask you to share your experience with any of those
application if there are any before this thread falls asleep.

First I try to show requirements. The project started with some people which
are somehow near by to each other, at least mainly. It is now about to grow and
there are plans to create independent nodes in some regions outside the
country of the headquarter.

So there will be some intensive and wide organization and collaboration
necessary what happens for many in their free time (what reminds me on Zulip's
statement about working in different time zones, see [Why
Zullip?](https://zulipchat.com/why-zulip/))

Moreover it needs some channels to speak to people outside the organization, in
regard of generic questions and asset specific questions.

Last but not least the platform has to coded, so code management has to
integrate as well.  So internally we need a app for collaboration and file
sharing, including some decent planning and management tools.  For the
externals we would like to avoid to use mainly emails (although there could be
ticket system behind), so I thought comment on our pages should be reused
for discussions like bugs or feature requests and meta data analysis.
Furthermore it would be welcome if they could reach us via well known chat apps
without the need to monitor and administer these apps separately.

It is totally clear that there is not a single application what can fulfill all
our requirements (at least yet). Thus besides being a mature application
(although not all of them in my list are so), it shall allow
[SSO](https://en.wikipedia.org/wiki/Single_sign-on) and available as container
image.

A good spot starting this research was [LisaDziuba/Awesome-Design-Tools: The
best design tools for everything][designtools] and [Which self hosted programs
do you use? — LowEndTalk][whichselfhosted] although it doesn't sound like the
right starting spot.  This repository is inspired by similar to the before
mentioned with inspiration from [Open Design: Freeware tools for creatives – UX
Planet][freewaretools] filled with answers to our requirements.

[designtools]: https://github.com/LisaDziuba/Awesome-Design-Tools
[whichselfhosted]: https://www.lowendtalk.com/discussion/118849/which-self-hosted-programs-do-you-use
[freewaretools]: https://uxplanet.org/open-design-freeware-tools-for-designers-f7bdde99f2e0
</details>

<details> 
  <summary><h2>Q2: why is there propertery software listed</h2></summary>
	At the beginning of your journey you focus to get your product done and properly don't have that much time to evaluation, set-up and administer software application as listed below. 
As we faced the same problem, we agreed to use a commercial product to get us organized and doing the evaluation etc. parallel, switching over step by step. 
</details>
## Team Chat (ex. Slack)

as Matrix, Mattermost and Rocket.Chat and Zulip are discussed most, here some sources I read:

 - [Timeto replace Slack! Who willwin, MatterMost orRiot/Matrix?](https://medium.com/ignation/time-to-replace-slack-who-will-win-mattermost-or-riot-matrix-a090e9cdc219)
- [It’stime to Riot(.im) – ToplBlog – Medium](https://medium.com/topl-blog/its-time-to-riot-im-8fb95eb39c9a)
- [Team Chat Recommendation: Mattermost, Riot, Zulip etc. I need low RAM consumption. : selfhosted](https://www.reddit.com/r/selfhosted/comments/9s5fzq/team_chat_recommendation_mattermost_riot_zulip/)
- why [Parity Technologies](https://www.parity.io/) switched to Matrix --> [why Team-Messenger:Ab in die Matrix! -Golem.de](https://www.golem.de/news/team-messenger-ab-in-die-matrix-1904-140850.html)


### Matrix

- **Home:** [Matrix.org](https://matrix.org/blog/index)
- **SSO:** yes ([This Week in Matrix 2018-11-26 |
  Matrix.org blog][matrix20181126])
- **Integrations:** many ([Try Matrix Now! | Matrix.org][trymatrix])
- **Deployment Images:** yes ([Guides | Matrix.org][guidesmatrix])
- **Remarks:**
  - it is pushed as:
    - [Matrix and Riot confirmed as the basis for France's Secure Instant
       Messenger app | Matrix.org blog][francesecure]
    - [FOSDEM 2019 - Matrix in the French State][fosdemmatrix]

[matrix20181126]: https://matrix.org/blog/2018/11/26/this-week-in-matrix-2018-11-26
[trymatrix]: https://matrix.org/docs/projects/try-matrix-now.html
[guidesmatrix]: https://matrix.org/docs/guides/
[francesecure]: https://matrix.org/blog/2018/04/26/matrix-and-riot-confirmed-as-the-basis-for-frances-secure-instant-messenger-app
[fosdemmatrix]: https://fosdem.org/2019/schedule/event/matrix_french_state/

<ul>
	<li>
		<a href="https://mattermost.com/nonprofit/" target="_blank" rel="nofollow noopener">Mattermost:Open Source, Private CloudSlack Alternative</a>
		<table>
			<tbody>
				<tr>
					<td style="text-align: center;">
						<strong>Integration</strong>
					</td>
					<td style="text-align: center;">
						<strong>Integrations</strong>
					</td>
					<td style="text-align: center;">
						<strong>Deploy Images</strong>
					</td>
					<td style="text-align: center;">
						<strong>Remark</strong>
					</td>
				</tr>
				<tr>
					<td valign="top">
						<a href="https://docs.mattermost.com/deployment/sso-saml.html" rel="nofollow">SSO</a> ok (but limteation to licencse)</td>
					<td valign="top">it offers <a href="https://integrations.mattermost.com/" rel="nofollow">a verycomprehensive collection of integrations</a>
					</td>
					<td valign="top">Docker etc. ok</td>
					<td valign="top">
					</td>
				</tr>
			</tbody>
		</table>
  <p>
  </p>
	</li>
	<li>
			<a href="https://rocket.chat/" target="_blank" rel="nofollow noopener">Rocket.Chat- Free, Open Source,Enterprise Team Chat</a>
		<table>
			<tbody>
				<tr>
					<td style="text-align: center;">
						<strong>Integration</strong>
					</td>
					<td style="text-align: center;">
						<strong>Integrations</strong>
					</td>
					<td style="text-align: center;">
						<strong>Deploy Images</strong>
					</td>
					<td style="text-align: center;">
						<strong>Remark</strong>
					</td>
				</tr>
				<tr>
					<td valign="top">
						<a href="https://rocket.chat/docs/administrator-guides/authentication/" rel="nofollow">SSO</a> ok</td>
					<td valign="top">it offers not that many <a href="https://rocket.chat/docs/administrator-guides/integrations/" rel="nofollow">integrations</a> as the others</td>
					<td valign="top"><a href="https://rocket.chat/install" rel="nofollow">Docker etc.</a> ok</td>
					<td valign="top">is very interesting in sense of collaboration as <a href="https://nextcloud.com/blog/rocket.chat-and-nextcloud-announce-partnership-and-integration/" rel="nofollow">Rocket.Chatand Nextcloud announcepartnership andintegration &ndash; Nextcloud</a>
					</td>
				</tr>
			</tbody>
		</table>
	</li>
	<li>
		<a href="https://zulipchat.com/" target="_blank" rel="nofollow noopener">Zulip - The world&rsquo;s most productive team chat</a>
		<table>
			<tbody>
				<tr>
					<td style="text-align: center;">
						<strong>Integration</strong>
					</td>
					<td style="text-align: center;">
						<strong>Integrations</strong>
					</td>
					<td style="text-align: center;">
						<strong>Deploy Images</strong>
					</td>
					<td style="text-align: center;">
						<strong>Remark</strong>
					</td>
				</tr>
				<tr>
					<td valign="top">
						<a href="https://zulipchat.com/security/" rel="nofollow">SSO</a>&nbsp;ok</td>
					<td valign="top">it offers <a href="https://integrations.mattermost.com/" rel="nofollow">a very large collectionof integrations</a>
					</td>
					<td valign="top">&nbsp;</td>
					<td valign="top">&nbsp;</td>
				</tr>
			</tbody>
		</table>
	</li>
	<li>
		<a href="http://muut.io/" target="_blank" rel="nofollow noopener">muut.io</a>
		<table>
			<tbody>
				<tr>
					<td style="text-align: center;">
						<strong>Integration</strong>
					</td>
					<td style="text-align: center;">
						<strong>Integrations</strong>
					</td>
					<td style="text-align: center;">
						<strong>Deploy Images</strong>
					</td>
					<td style="text-align: center;">
						<strong>Remark</strong>
					</td>
				</tr>
				<tr>
					<td valign="top">?</td>
					<td valign="top">it offers <a href="https://integrations.mattermost.com/" rel="nofollow">a very large collectionof integrations</a>
					</td>
					<td valign="top">hosted, builder or <a href="https://muut.com/forum/#!/moot/setting-up:free-version" rel="nofollow">FreeVersion | Muut community</a>
					</td>
					<td valign="top">&nbsp;</td>
				</tr>
			</tbody>
		</table>
	</li>
</ul>

5. Forum / Notes / documentation

6. 1. [Start | Read the Docs](https://readthedocs.org/)

   2. [Discourse  - Civilized Discussion ](https://www.discourse.org/)
    --> can be embedded [UsingDiscourse to powercomments in an eventsystem or blog?](https://meta.discourse.org/t/using-discourse-to-power-comments-in-an-event-system-or-blog/90308)[,    Embedding Discourse    Comments via    Javascript](https://meta.discourse.org/t/embedding-discourse-comments-via-javascript/31963),
      -->[Official  Single-Sign-On for  Discourse (sso)](https://meta.discourse.org/t/official-single-sign-on-for-discourse-sso/13045)
      --> [Chat  Integration](https://www.discourse.org/plugins/chat-integration.html)
    --> kind of [sitechat](https://discourse-shoutbox.info/) and [Babble- A Chat Plugin - plugin -Discourse Meta](https://meta.discourse.org/t/babble-a-chat-plugin/87297)

   3. Flarum
    --> can be [EmbedFlarum Comments ViaJavaScript?](https://discuss.flarum.org/d/882-embed-flarum-comments-via-javascript),
    --> site chat  [How to useFlarum like Disqus addchat & login on Blog ?
    ](https://discuss.flarum.org/d/14997-how-to-use-flarum-like-disqus-add-chat-login-on-blog)--> [SingleSign On](https://discuss.flarum.org/d/5052-single-sign-on)

7. - a little help for orientation -> [Which is    Better? Discourse or    Flarum?](https://meta.discourse.org/t/which-is-better-discourse-or-flarum/71726)


8. 1. [Take aboard to collaborate withothers | board.net](http://board.net/)



9. [disqus](https://disqus.com/) - commenting plug-in

10. 1. [Isso – acommenting server similarto Disqus](https://posativ.org/isso/)

    2. [HostedComments Service |Remarkbox](https://www.remarkbox.com/)

    3. [rocket.chat-> embedded layout](https://rocket.chat/docs/developer-guides/embedded-layout/)


    4. [Babble- A Chat Plugin - plugin -Discourse Meta](https://meta.discourse.org/t/babble-a-chat-plugin/87297)

    5. some sources I read

    6. 1. <https://www.slant.co/options/622/alternatives/~disqus-alternatives>
       2. [Disqus  Alternatives - tips  & tricks - Hugo  Discussion](https://discourse.gohugo.io/t/disqus-alternatives/2948)
       3. <https://victorzhou.com/blog/replacing-disqus/>



11. [Freshdesk](https://freshdesk.com/), [Zendesk](https://www.zendesk.com/) - ticket system & customer support

12. 1. [osTicket |Support Ticketing System](https://osticket.com/),    [SSO](https://forum.osticket.com/d/85191-sso-implementation) ok   , Docker ok

    2. [OpenSource Helpdesk System foreCommerce, Marketplaces& Multichannel -UVdesk](https://www.uvdesk.com/en/opensource-features/)



13. [Basecamp](https://basecamp.com/) ([partly   open source](https://basecamp.com/about/open-source)), [Jira](https://www.atlassian.com/software/jira)&Trello, [Wrike](https://www.wrike.com/) - project management

Sources:
  1. [Is there a resource planning tool you can recommend for nethserver?](https://community.nethserver.org/t/is-there-a-resource-planning-tool-you-can-recommend-for-nethserver/6941)

Apps:
   1. [Taiga.io](https://taiga.io/),   SSO (?), [Taiga:Other ways to setupinitial environment](https://taigaio.github.io/taiga-doc/dist/setup-alternatives.html)
   2. [EnterpriseOpen Source ProjectManagement Software |Features | OrangeScrum](https://www.orangescrum.org/)
   3. [OpenProject- online projectmanagement software - freeand open source](https://www.openproject.org/)
   4. [Twproject - Project management software, time tracking software](https://twproject.com/)
   4. [Freedcamp- Free Project Management](https://freedcamp.com/)
   5. [Wekan— open-source kanban](https://wekan.github.io/)
   6. [Nextcloud](https://nextcloud.com/), but only with limitations, see  [Tasks & Calendar extended to be used as project management tool](https://help.nextcloud.com/t/tasks-calendar-extended-to-be-used-as-project-management-tool/1274) and [Calendar / Tasks in SIMPLE project management](https://help.nextcloud.com/t/calendar-tasks-in-simple-project-management/6993/8)
   7. with limitations: [Bitrix24:#1 Free CollaborationPlatform With CRM, Tasks,Projects, Documents,Messaging And Much More](https://www.bitrix24.com/)



15. DropBox - File Hosting, collaboration  and more


16. 1. [Nextcloud](https://nextcloud.com/),   [SSO](https://apps.nextcloud.com/apps/user_saml) ok,   [Dockeretc](https://nextcloud.com/install/#instructions-server) ok
    2. [ownCloud -The leading OpenSourceCloud CollaborationPlatform.](https://owncloud.org/)
    3. [GroupOffice - An open sourceCRM and groupwareapplication](https://www.group-office.com)
    4. [Home | Open-Xchange](https://www.open-xchange.com/)
    5. [Open Source Collaboration Software - Future Teamwork | Kopano](https://kopano.com/)



17. [Mapbox](https://www.mapbox.com/) - asset location visualization


18. 1. ?



19. Natural Language Processing


20. 1. [Apertium | A free/open-source machinetranslation platform](https://www.apertium.org)

    2. [THUNLP-MT/THUMT:An open-source neuralmachine translationtoolkit developed byTsinghua Natural LanguageProcessing Group](https://github.com/THUNLP-MT/THUMT)
    3. deepl.com (partly free but   a way better than google,   saved my life several times)
    4. ([FrameNet](https://framenet.icsi.berkeley.edu/fndrupal/about))
