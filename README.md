# DeepaMehta 5 search/create widget

## Version History

**0.20** -- Dec 21, 2018

* Show type icons in "Create" menu
* Revise "Create" menu (option groups)
* Retype component property `menu-topic-types` to Array (formerly Object) to support sort order

**0.19** -- Nov 24, 2018

* Improvement: debounce search requests

**0.18** -- Oct 21, 2018

* Return to no-tabs layout

**0.17** -- Oct 6, 2018

* New component property `markerIds` allows rendering certain search result topics as "marked"
* Component supports manual mounting in conjunction with manual data update ("props" are mirrored as "data")
* Fix: update search result on show dialog

**0.16** -- Sep 30, 2018

* New component prop `createEnabled` controls whether the "Create" tab is enabled

**0.15** -- Aug 22, 2018

* Composability:
    * The component emits events instead of dispatching into the host application. Events and their args:
        * `topic-reveal`  topic
        * `topic-create`  {topicType, value}
        * `extra-create`  {extraItem, value, optionsData}
        * `close`         -
    * The component receives app state via props instead of maintaining a Vuex store module on its own.
        * No Vuex dependency anymore

**0.14** -- Aug 18, 2018

* Pass widget `pos` to extra menu item `create` callback
* Fix: process directives on create-topic

**0.13** -- Jul 31, 2018

* Add GitLab CI/CD

**0.12** -- May 1, 2018

* Adapt Element UI overrides

**0.11** -- Apr 10, 2018

* 2-tab layout: "Search" and "Create"

**0.10** -- Mar 25, 2018

* New concept: the extra menu items can provide a "Create Options Component" to solicit further data from the user before creating the topic.
* Dependencies: `dm5-topic-list` replaces `el-table` as the result list component. Build size decreases by 100 KiB!

**0.9** -- Mar 22, 2018

* New option `topicHandler` replaces `auxAction`. Allows the handler and the `openSearchWidget` call to exist in the same closure.

**0.8** -- Jan 13, 2018

* Minor layout change

**0.7** -- Dec 5, 2017

* Adapt to Element UI 2.0

**0.6** -- Oct 19, 2017

* Incremental injection of extra items into type menu (via action)

**0.5** -- Oct 3, 2017

* Parent component can add extra items to type menu

**0.4** -- Sep 7, 2017

* 2 new options: `noSelect` and `auxAction`

**0.3** -- Jul 17, 2017

**0.2** -- Jun 30, 2017

**0.1** -- Jun 14, 2017

------------
Jörg Richter  
Dec 21, 2018
