# macos-27
macos 27<ntp-app realbox-can-show-secondary-side="" modules-loaded-status_="2" energy-effect-enabled_="" energy-effect-animation-enabled_="" energy-effect-variant_="energy-effect-fusebox" show-background-image_="" style="--ntp-logo-color: rgba(238, 238, 238, 1.00); --color-new-tab-page-attribution-foreground: rgba(248, 249, 250, 1.00); --color-new-tab-page-most-visited-foreground: rgba(248, 249, 250, 1.00);" modules-shown-to-user=""><template shadowrootmode="open"><!----><!--_html_template_start_--><!-- #html_wrapper_imports_start
import {SubmitButtonIconType} from '//resources/cr_components/composebox/composebox.js';
#html_wrapper_imports_end -->
<div id="content">
  <!--?lit$616380449$-->
  <div id="rhsWrapper">
    <div id="rhsContent">
      <!--?lit$616380449$-->
      <!--?lit$616380449$-->
        <!--?lit$616380449$-->
          <div id="oneGoogleBarScrim" fixed=""></div>
          <ntp-iframe id="oneGoogleBar" src="chrome-untrusted://new-tab-page/one-google-bar?paramsencoded=" allow="" style="clip-path: url(&quot;#oneGoogleBarClipPath&quot;); z-index: 1000;"><template shadowrootmode="open"><!----><!--_html_template_start_--><!-- #html_wrapper_imports_start
import {nothing} from '//resources/lit/v3_0/lit.rollup.js';
#html_wrapper_imports_end -->
<iframe id="iframe" src="chrome-untrusted://new-tab-page/one-google-bar?paramsencoded=">
</iframe>
<!--_html_template_end_--></template>
          </ntp-iframe>
        
      
      <!-- TODO(crbug.com/40743294): Instead of ?hidden="${!this.logoEnabled_}" it would
          be nicer to use Lit's conditional rendering. However, that breaks
          StartupBrowserCreatorPickerNoParamsTest.ShowPickerWhenAlreadyLaunched on
          the msan builder. See crbug.com/40743659. -->
      <ntp-logo id="logo" show-tight-doodle-boxing_="" use-google-logo26_="" single-colored=""><template shadowrootmode="open"><!----><!--_html_template_start_--><!--?lit$616380449$-->
  <div id="logo"></div>

<!--?lit$616380449$-->
<!--?lit$616380449$-->
<!--_html_template_end_--></template>
      </ntp-logo>
      <!--?lit$616380449$-->
      <div id="searchboxContainer">
        <ntp-searchbox id="searchbox" placeholder-text="Search Google or type a URL" can-show-secondary-side="" compose-button-enabled="" searchbox-layout-mode="" context-menu-glif-animation-state="ineligible" animation-state="" searchbox-voice-search-enabled_="" searchbox-lens-search-enabled_="" use-webkit-search-icons_="" shown=""><template shadowrootmode="open"><!----><!--_html_template_start_-->
<div id="inputWrapper">
  <!--?lit$616380449$-->
  <cr-searchbox-input id="input" exportparts="searchbox-input" placeholder-text="Search Google or type a URL" searchbox-aria-description="" searchbox-icon="//resources/cr_components/searchbox/icons/search_cr23.svg"><template shadowrootmode="open"><!----><!--_html_template_start_-->
<div id="inputInnerContainer" part="input-inner-container">
    <slot name="contextual-entrypoint"></slot>
    <cr-searchbox-icon id="icon" in-searchbox="" part="icon" aria-hidden="true" page-url="" default-icon="//resources/cr_components/searchbox/icons/search_cr23.svg" mask-image="url(//resources/cr_components/searchbox/icons/search_cr23.svg)" favicon-image_=""><template shadowrootmode="open"><!----><!--_html_template_start_-->
<div id="container" aria-hidden="true" style="--container-bg-color:transparent;">
  <img id="image" alt="" src="" hidden="">

  <div>
    <div id="icon" style="-webkit-mask-image: url(//resources/cr_components/searchbox/icons/search_cr23.svg);">
    </div>
    <div id="faviconImageContainer" hidden="">
      <img id="faviconImage" alt="" src="" srcset="">
    </div>
  </div>

  <img id="iconImg" alt="" src="" hidden="">
</div>
<!--_html_template_end_--></template>
    </cr-searchbox-icon>
    <slot name="thumbnail"></slot>
    <!--?lit$616380449$-->
    <!-- Target of the input's aria-activedescendant while a selection is
         active. It distracts screen readers from the input's value, which
         previews the selection, so the notification of the selection's label
         wins over the value change. Must share the input's shadow root for
         element reflection to work. It is an option of a listbox the combobox
         controls because that is the one kind of active descendant VoiceOver
         accepts as keyboard focus after a key press: told that focus is on a
         plain group, it re-anchors keyboard focus on the web area, which blurs
         the input and closes the popup, whatever the group's position or
         focusability. Hidden, hence out of the accessibility tree, while there
         is no selection (see setSelectionA11yLabel()). -->
    <div id="selectionListbox" role="listbox" hidden="">
      <div id="selectionAnnouncement" role="option" aria-selected="true"></div>
    </div>
    <div id="mirrorContainer">
      <div id="mirror" part="mirror" aria-hidden="true" hidden=""></div>
      <!--?lit$616380449$-->
        <input id="input" class="truncate" type="search" autocomplete="off" part="searchbox-input" spellcheck="false" role="combobox" aria-controls="selectionListbox" aria-expanded="false" aria-description="" placeholder="Search Google or type a URL">
      
    </div>
    <span id="ellipsisIndicator" aria-hidden="true">...</span>
    <slot name="action-buttons"></slot>
    <slot name="compose-button"></slot>
</div>
<!--_html_template_end_--></template>
    <!--?lit$616380449$-->
    <!--?lit$616380449$-->
      <div slot="action-buttons" class="searchbox-icon-button-container voice">
        <button id="voiceSearchButton" class="searchbox-icon-button" tabindex="0" title="Search by voice">
        </button>
      </div>
    
    <!--?lit$616380449$-->
      <div slot="action-buttons" class="searchbox-icon-button-container lens">
        <button id="lensSearchButton" class="searchbox-icon-button lens" tabindex="0" title="Search by image">
        </button>
      </div>
    
    <!--?lit$616380449$-->
      <cr-searchbox-compose-button id="composeButton" slot="compose-button" label-text="AI Mode" tooltip-title="Ask AI Mode in Google Search" a11y-label="Ask AI Mode in Google Search" compose-icon="//resources/cr_components/searchbox/icons/search_spark.svg" energy-effect-animation-enabled=""><template shadowrootmode="open"><!----><!--_html_template_start_-->
<div id="glowAnimationWrapper" class="glow-container" part="glow-container">
  <!--?lit$616380449$-->
  <div class="input-plate-gradient">
    <div class="input-plate-gradient-mask">
      <div class="gradient-blur-wrapper">
        <div class="gradient-mask">
          <div class="gradient"></div>
        </div>
      </div>
      <div class="gradient-blur-wrapper sharp-tip">
        <div class="gradient-mask">
          <div class="gradient"></div>
        </div>
      </div>
    </div>
  </div>
  <cr-button id="composeButton" class="compose-container" part="compose-button" exportparts="hoverBackground" tabindex="0" aria-label="Ask AI Mode in Google Search" title="Ask AI Mode in Google Search" role="button" aria-disabled="false" has-prefix-icon_="" has-suffix-icon_=""><template shadowrootmode="open"><!---->
<div id="background"></div>
<slot id="prefixIcon" name="prefix-icon">
</slot>
<span id="content">
  <slot></slot>
</span>
<slot id="suffixIcon" name="suffix-icon">
</slot>
<div id="hoverBackground" part="hoverBackground"></div></template>
    <!--?lit$616380449$-->
    <div slot="prefix-icon" class="compose-icon" part="compose-icon" style="-webkit-mask-image: url(//resources/cr_components/searchbox/icons/search_spark.svg);
               mask-image: url(//resources/cr_components/searchbox/icons/search_spark.svg);">
    </div>
    
    <span id="label" part="label"><!--?lit$616380449$-->AI Mode</span>
    <div id="arrowIcon" slot="suffix-icon" class="arrow-icon" part="arrow-icon" style="-webkit-mask-image: url(//resources/cr_components/searchbox/icons/arrow_forward.svg);
               mask-image: url(//resources/cr_components/searchbox/icons/arrow_forward.svg);">
    </div>
  </cr-button>
</div>
<!--_html_template_end_--></template>
      </cr-searchbox-compose-button>
    
  </cr-searchbox-input>
  <div class="dropdownContainer">
    <cr-searchbox-dropdown id="matches" part="searchbox-dropdown" exportparts="dropdown-content" role="listbox" selected-match-index="-1" can-show-secondary-side="" hidden=""><template shadowrootmode="open"><!----><!--_html_template_start_-->
<div id="content" part="dropdown-content">
<!--?lit$616380449$--><!---->
  <div class="primary-side">
    <!--?lit$616380449$-->
  </div>
<!---->
</div>
<!--_html_template_end_--></template>
    </cr-searchbox-dropdown>
  </div>
</div>
<!--_html_template_end_--></template>
        </ntp-searchbox>
        <div id="dialogAnchor"></div>
        <!--?lit$616380449$-->
        <!--?lit$616380449$-->
      </div>
      <!--?lit$616380449$-->
      <!--?lit$616380449$-->
        <cr-toast id="webstoreToast" duration="10000" hidden=""><template shadowrootmode="open"><!----><slot></slot></template>
          <div>You can find older colours in the Chrome Web Store</div>
          <cr-button role="button" tabindex="0" aria-disabled="false"><template shadowrootmode="open"><!---->
<div id="background"></div>
<slot id="prefixIcon" name="prefix-icon">
</slot>
<span id="content">
  <slot></slot>
</span>
<slot id="suffixIcon" name="suffix-icon">
</slot>
<div id="hoverBackground" part="hoverBackground"></div></template>
            Find themes
          </cr-button>
        </cr-toast>
      
      <!--?lit$616380449$-->
        <!--?lit$616380449$-->
          <cr-most-visited id="mostVisited" single-row="" reflow-on-overflow="" max-tiles-in-collapsed-state="6" max-shortcuts-in-expanded-state="10" max-most-visited-tiles-in-expanded-state="8" max-enterprise-shortcuts="10" is-dark_="" max-tiles="0" visible_="" custom-links-enabled_=""><template shadowrootmode="open"><!----><!--_html_template_start_-->
<div id="container" style="--tile-background-color: rgba(230, 233, 243, 1.00); --column-count: 4; --row-count: 1;">
  <!--?lit$616380449$--><!---->
    <div class="tile" title="inbox" draggable="true" data-index="0">
      <a draggable="false" href="https://gmail.com/" aria-label="inbox"></a>
      <cr-icon-button id="actionMenuButton" class="icon-more-vert" tabindex="0" title="More actions for inbox shortcut" data-index="0" role="button" aria-disabled="false"><template shadowrootmode="open"><!---->
<div id="icon">
  <div id="maskedImage"></div>
</div></template>
      </cr-icon-button>
      <cr-icon-button id="removeButton" class="icon-clear" tabindex="0" title="Remove inbox" hidden="" data-index="0" role="button" aria-disabled="false"><template shadowrootmode="open"><!---->
<div id="icon">
  <div id="maskedImage"></div>
</div></template>
      </cr-icon-button>
      <div class="tile-icon">
        <img draggable="false" alt="" src="chrome://favicon2/?size=24&amp;scaleFactor=1x&amp;showFallbackMonogram=&amp;pageUrl=https%3A%2F%2Fgmail.com%2F">
        <div class="query-tile-icon" draggable="false" hidden="">
        </div>
        <div class="managed-tile-icon" hidden="">
          <cr-policy-indicator indicator-type="userPolicy"><template shadowrootmode="open"><!---->
<cr-tooltip-icon tooltip-text="" icon-class="cr20:domain" icon-aria-label="" tooltip-position="top"><template shadowrootmode="open"><!---->
<cr-icon id="indicator" tabindex="0" aria-describedby="tooltip" role="img" aria-label="" icon="cr20:domain"><template shadowrootmode="open"><svg id="baseSvg" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid meet" focusable="false" viewBox="0 0 20 20" class="cr-iconset-svg-icon_" style="display: block; height: 100%; width: 100%; pointer-events: none;">
<g>
        <path d="M2 15.5v-11c0-.414.148-.766.441-1.059A1.443 1.443 0 0 1 3.5 3h5c.414 0 .766.148 1.059.441.293.293.441.645.441 1.059V6h6.5c.414 0 .766.148 1.059.441.293.293.441.645.441 1.059v8c0 .414-.148.766-.441 1.059A1.443 1.443 0 0 1 16.5 17h-13c-.414 0-.766-.148-1.059-.441A1.443 1.443 0 0 1 2 15.5Zm1.5 0H5V14H3.5Zm0-3.168H5v-1.5H3.5Zm0-3.164H5v-1.5H3.5ZM3.5 6H5V4.5H3.5ZM7 15.5h1.5V14H7Zm0-3.168h1.5v-1.5H7Zm0-3.164h1.5v-1.5H7ZM7 6h1.5V4.5H7Zm3 9.5h6.5v-8H10v1.668h1.5v1.5H10v1.664h1.5v1.5H10Zm3.5-4.832v-1.5H15v1.5Zm0 3.164v-1.5H15v1.5Zm0 0"></path>
      </g></svg><!----></template>
</cr-icon>
<cr-tooltip id="tooltip" for="indicator" fit-to-visible-bounds="" part="tooltip" position="top" style="--paper-tooltip-delay-in: 500ms; --cr-tooltip-offset: 14px;"><template shadowrootmode="open"><!---->
<div id="tooltip" hidden="" part="tooltip">
  <slot></slot>
</div>
<div id="tooltipOffsetFiller"></div></template>
  <slot name="tooltip-text"><!--?lit$616380449$--></slot>
</cr-tooltip></template>
</cr-tooltip-icon></template>
          </cr-policy-indicator>
        </div>
      </div>
      <div class="tile-title title-ltr">
        <span><!--?lit$616380449$-->inbox</span>
      </div>
    </div>
  <!----><!---->
    <div class="tile" title="reading eggs" draggable="true" data-index="1">
      <a draggable="false" href="https://student.readingeggspress.com/" aria-label="reading eggs"></a>
      <cr-icon-button id="actionMenuButton" class="icon-more-vert" tabindex="0" title="More actions for reading eggs shortcut" data-index="1" role="button" aria-disabled="false"><template shadowrootmode="open"><!---->
<div id="icon">
  <div id="maskedImage"></div>
</div></template>
      </cr-icon-button>
      <cr-icon-button id="removeButton" class="icon-clear" tabindex="0" title="Remove reading eggs" hidden="" data-index="1" role="button" aria-disabled="false"><template shadowrootmode="open"><!---->
<div id="icon">
  <div id="maskedImage"></div>
</div></template>
      </cr-icon-button>
      <div class="tile-icon">
        <img draggable="false" alt="" src="chrome://favicon2/?size=24&amp;scaleFactor=1x&amp;showFallbackMonogram=&amp;pageUrl=https%3A%2F%2Fstudent.readingeggspress.com%2F">
        <div class="query-tile-icon" draggable="false" hidden="">
        </div>
        <div class="managed-tile-icon" hidden="">
          <cr-policy-indicator indicator-type="userPolicy"><template shadowrootmode="open"><!---->
<cr-tooltip-icon tooltip-text="" icon-class="cr20:domain" icon-aria-label="" tooltip-position="top"><template shadowrootmode="open"><!---->
<cr-icon id="indicator" tabindex="0" aria-describedby="tooltip" role="img" aria-label="" icon="cr20:domain"><template shadowrootmode="open"><svg id="baseSvg" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid meet" focusable="false" viewBox="0 0 20 20" class="cr-iconset-svg-icon_" style="display: block; height: 100%; width: 100%; pointer-events: none;">
<g>
        <path d="M2 15.5v-11c0-.414.148-.766.441-1.059A1.443 1.443 0 0 1 3.5 3h5c.414 0 .766.148 1.059.441.293.293.441.645.441 1.059V6h6.5c.414 0 .766.148 1.059.441.293.293.441.645.441 1.059v8c0 .414-.148.766-.441 1.059A1.443 1.443 0 0 1 16.5 17h-13c-.414 0-.766-.148-1.059-.441A1.443 1.443 0 0 1 2 15.5Zm1.5 0H5V14H3.5Zm0-3.168H5v-1.5H3.5Zm0-3.164H5v-1.5H3.5ZM3.5 6H5V4.5H3.5ZM7 15.5h1.5V14H7Zm0-3.168h1.5v-1.5H7Zm0-3.164h1.5v-1.5H7ZM7 6h1.5V4.5H7Zm3 9.5h6.5v-8H10v1.668h1.5v1.5H10v1.664h1.5v1.5H10Zm3.5-4.832v-1.5H15v1.5Zm0 3.164v-1.5H15v1.5Zm0 0"></path>
      </g></svg><!----></template>
</cr-icon>
<cr-tooltip id="tooltip" for="indicator" fit-to-visible-bounds="" part="tooltip" position="top" style="--paper-tooltip-delay-in: 500ms; --cr-tooltip-offset: 14px;"><template shadowrootmode="open"><!---->
<div id="tooltip" hidden="" part="tooltip">
  <slot></slot>
</div>
<div id="tooltipOffsetFiller"></div></template>
  <slot name="tooltip-text"><!--?lit$616380449$--></slot>
</cr-tooltip></template>
</cr-tooltip-icon></template>
          </cr-policy-indicator>
        </div>
      </div>
      <div class="tile-title title-ltr">
        <span><!--?lit$616380449$-->reading eggs</span>
      </div>
    </div>
  <!----><!---->
    <div class="tile" title="Exhibition group 7 checklist for Omer" draggable="true" data-index="2">
      <a draggable="false" href="https://www.canva.com/design/DAHQn-QjuDM/ciRiaKE3bQu87YhpgYcQlw/edit" aria-label="Exhibition group 7 checklist for Omer"></a>
      <cr-icon-button id="actionMenuButton" class="icon-more-vert" tabindex="0" title="More actions for Exhibition group 7 checklist for Omer shortcut" data-index="2" role="button" aria-disabled="false"><template shadowrootmode="open"><!---->
<div id="icon">
  <div id="maskedImage"></div>
</div></template>
      </cr-icon-button>
      <cr-icon-button id="removeButton" class="icon-clear" tabindex="0" title="Remove Exhibition group 7 checklist for Omer" hidden="" data-index="2" role="button" aria-disabled="false"><template shadowrootmode="open"><!---->
<div id="icon">
  <div id="maskedImage"></div>
</div></template>
      </cr-icon-button>
      <div class="tile-icon">
        <img draggable="false" alt="" src="chrome://favicon2/?size=24&amp;scaleFactor=1x&amp;showFallbackMonogram=&amp;pageUrl=https%3A%2F%2Fwww.canva.com%2Fdesign%2FDAHQn-QjuDM%2FciRiaKE3bQu87YhpgYcQlw%2Fedit">
        <div class="query-tile-icon" draggable="false" hidden="">
        </div>
        <div class="managed-tile-icon" hidden="">
          <cr-policy-indicator indicator-type="userPolicy"><template shadowrootmode="open"><!---->
<cr-tooltip-icon tooltip-text="" icon-class="cr20:domain" icon-aria-label="" tooltip-position="top"><template shadowrootmode="open"><!---->
<cr-icon id="indicator" tabindex="0" aria-describedby="tooltip" role="img" aria-label="" icon="cr20:domain"><template shadowrootmode="open"><svg id="baseSvg" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid meet" focusable="false" viewBox="0 0 20 20" class="cr-iconset-svg-icon_" style="display: block; height: 100%; width: 100%; pointer-events: none;">
<g>
        <path d="M2 15.5v-11c0-.414.148-.766.441-1.059A1.443 1.443 0 0 1 3.5 3h5c.414 0 .766.148 1.059.441.293.293.441.645.441 1.059V6h6.5c.414 0 .766.148 1.059.441.293.293.441.645.441 1.059v8c0 .414-.148.766-.441 1.059A1.443 1.443 0 0 1 16.5 17h-13c-.414 0-.766-.148-1.059-.441A1.443 1.443 0 0 1 2 15.5Zm1.5 0H5V14H3.5Zm0-3.168H5v-1.5H3.5Zm0-3.164H5v-1.5H3.5ZM3.5 6H5V4.5H3.5ZM7 15.5h1.5V14H7Zm0-3.168h1.5v-1.5H7Zm0-3.164h1.5v-1.5H7ZM7 6h1.5V4.5H7Zm3 9.5h6.5v-8H10v1.668h1.5v1.5H10v1.664h1.5v1.5H10Zm3.5-4.832v-1.5H15v1.5Zm0 3.164v-1.5H15v1.5Zm0 0"></path>
      </g></svg><!----></template>
</cr-icon>
<cr-tooltip id="tooltip" for="indicator" fit-to-visible-bounds="" part="tooltip" position="top" style="--paper-tooltip-delay-in: 500ms; --cr-tooltip-offset: 14px;"><template shadowrootmode="open"><!---->
<div id="tooltip" hidden="" part="tooltip">
  <slot></slot>
</div>
<div id="tooltipOffsetFiller"></div></template>
  <slot name="tooltip-text"><!--?lit$616380449$--></slot>
</cr-tooltip></template>
</cr-tooltip-icon></template>
          </cr-policy-indicator>
        </div>
      </div>
      <div class="tile-title title-ltr">
        <span><!--?lit$616380449$-->Exhibition group 7 checklist for Omer</span>
      </div>
    </div>
  <!---->
  <cr-button id="addShortcut" tabindex="0" noink="" aria-label="Add shortcut" title="Add shortcut" role="button" aria-disabled="false"><template shadowrootmode="open"><!---->
<div id="background"></div>
<slot id="prefixIcon" name="prefix-icon">
</slot>
<span id="content">
  <slot></slot>
</span>
<slot id="suffixIcon" name="suffix-icon">
</slot>
<div id="hoverBackground" part="hoverBackground"></div></template>
    <div class="tile-icon tile-icon-container">
      <div id="addShortcutIcon" draggable="false"></div>
    </div>
    <div class="tile-title">
      <span><!--?lit$616380449$-->Add shortcut</span>
    </div>
  </cr-button>
  <div>
    <cr-button id="showMore" tabindex="0" noink="" hidden="" aria-label="Show more" title="Show more" role="button" aria-disabled="false"><template shadowrootmode="open"><!---->
<div id="background"></div>
<slot id="prefixIcon" name="prefix-icon">
</slot>
<span id="content">
  <slot></slot>
</span>
<slot id="suffixIcon" name="suffix-icon">
</slot>
<div id="hoverBackground" part="hoverBackground"></div></template>
      <div class="tile-icon tile-icon-container">
        <div id="showMoreIcon" draggable="false"></div>
      </div>
      <div class="tile-title">
        <span><!--?lit$616380449$-->Show more</span>
      </div>
    </cr-button>
    <cr-button id="showLess" tabindex="0" noink="" hidden="" aria-label="Show less" title="Show less" role="button" aria-disabled="false"><template shadowrootmode="open"><!---->
<div id="background"></div>
<slot id="prefixIcon" name="prefix-icon">
</slot>
<span id="content">
  <slot></slot>
</span>
<slot id="suffixIcon" name="suffix-icon">
</slot>
<div id="hoverBackground" part="hoverBackground"></div></template>
      <div class="tile-icon tile-icon-container">
        <div id="showLessIcon" draggable="false"></div>
      </div>
      <div class="tile-title">
        <span><!--?lit$616380449$-->Show less</span>
      </div>
    </cr-button>
  </div>
  <cr-dialog id="dialog" consume-keydown-event=""><template shadowrootmode="open"><!---->
<dialog id="dialog" part="dialog" aria-labelledby="title">
  <!-- This wrapper is necessary, such that the "pulse" animation is not
    erroneously played when the user clicks on the outer-most scrollbar. -->
  <div id="content-wrapper" part="wrapper">
    <div class="top-container">
      <h2 id="title" class="title-container" tabindex="-1">
        <slot name="title"></slot>
      </h2>
      <!--?lit$616380449$-->
    </div>
    <slot name="header"></slot>
    <div class="body-container cr-scrollable" id="container" part="body-container">
      <div class="cr-scrollable-top"></div>
      <slot name="body"></slot>
      <div class="cr-scrollable-bottom"></div>
    </div>
    <slot name="button-container"></slot>
    <slot name="footer"></slot>
  </div>
</dialog></template>
    <div slot="title"><!--?lit$616380449$--></div>
    <div slot="body" id="dialogContent">
      <!--?lit$616380449$-->
      <cr-input id="dialogInputName" spellcheck="false" autofocus="" label="Name"><template shadowrootmode="open"><!---->
<div id="label" class="cr-form-field-label">
  <!--?lit$616380449$-->Name
</div>
<div id="row-container" part="row-container">
  <div id="input-container">
    <div id="inner-input-container">
      <div id="hover-layer"></div>
      <div id="inner-input-content">
        <slot name="inline-prefix"></slot>
        <input id="input" part="input" autocomplete="off" autofocus="" tabindex="0" type="text" maxlength="" minlength="" inputmode="" aria-labelledby="label" aria-label="Name" aria-invalid="false">
        <slot name="inline-suffix"></slot>
      </div>
    </div>
    <div id="underline-base"></div>
    <div id="underline"></div>
  </div>
  <slot name="suffix"></slot>
</div>
<div id="error" aria-live="assertive"><!--
  --><!--?lit$616380449$--><!--
--></div></template>
      </cr-input>
      <cr-input id="dialogInputUrl" spellcheck="false" type="url" label="URL"><template shadowrootmode="open"><!---->
<div id="label" class="cr-form-field-label">
  <!--?lit$616380449$-->URL
</div>
<div id="row-container" part="row-container">
  <div id="input-container">
    <div id="inner-input-container">
      <div id="hover-layer"></div>
      <div id="inner-input-content">
        <slot name="inline-prefix"></slot>
        <input id="input" part="input" autocomplete="off" tabindex="0" type="url" maxlength="" minlength="" inputmode="" aria-labelledby="label" aria-label="URL" aria-invalid="false">
        <slot name="inline-suffix"></slot>
      </div>
    </div>
    <div id="underline-base"></div>
    <div id="underline"></div>
  </div>
  <slot name="suffix"></slot>
</div>
<div id="error" aria-live="assertive"><!--
  --><!--?lit$616380449$--><!--
--></div></template>
      </cr-input>
    </div>
    <div slot="button-container">
      <cr-button class="cancel-button" role="button" tabindex="0" aria-disabled="false"><template shadowrootmode="open"><!---->
<div id="background"></div>
<slot id="prefixIcon" name="prefix-icon">
</slot>
<span id="content">
  <slot></slot>
</span>
<slot id="suffixIcon" name="suffix-icon">
</slot>
<div id="hoverBackground" part="hoverBackground"></div></template>
        <!--?lit$616380449$-->Cancel
      </cr-button>
      <cr-button class="action-button" disabled="" role="button" tabindex="-1" aria-disabled="true"><template shadowrootmode="open"><!---->
<div id="background"></div>
<slot id="prefixIcon" name="prefix-icon">
</slot>
<span id="content">
  <slot></slot>
</span>
<slot id="suffixIcon" name="suffix-icon">
</slot>
<div id="hoverBackground" part="hoverBackground"></div></template>
        <!--?lit$616380449$-->Done
      </cr-button>
    </div>
  </cr-dialog>
  <cr-action-menu id="actionMenu"><template shadowrootmode="open"><!---->
<dialog id="dialog" part="dialog" role="application">
  <div id="wrapper" class="item-wrapper" role="menu" tabindex="-1">
    <slot id="contentNode"></slot>
  </div>
</dialog></template>
    <button id="actionMenuViewOrEdit" class="dropdown-item" role="menuitem">
      <!--?lit$616380449$-->
    </button>
    <!--?lit$616380449$-->
    <button id="actionMenuRemove" class="dropdown-item" role="menuitem">
      <!--?lit$616380449$-->Remove
    </button>
  </cr-action-menu>
</div>
<cr-toast-manager id="toastManager" duration="10000"><template shadowrootmode="open"><!---->
<cr-toast id="toast"><template shadowrootmode="open"><!----><slot></slot></template>
  <div id="content" class="elided-text"></div>
  <slot id="slotted"></slot>
</cr-toast></template>
  <cr-button id="undo" aria-label="Press ⌘Z to undo" role="button" tabindex="0" aria-disabled="false"><template shadowrootmode="open"><!---->
<div id="background"></div>
<slot id="prefixIcon" name="prefix-icon">
</slot>
<span id="content">
  <slot></slot>
</span>
<slot id="suffixIcon" name="suffix-icon">
</slot>
<div id="hoverBackground" part="hoverBackground"></div></template>
    <!--?lit$616380449$-->Undo
  </cr-button>
  <cr-button id="restore" aria-label="Restore default shortcuts" role="button" tabindex="0" aria-disabled="false"><template shadowrootmode="open"><!---->
<div id="background"></div>
<slot id="prefixIcon" name="prefix-icon">
</slot>
<span id="content">
  <slot></slot>
</span>
<slot id="suffixIcon" name="suffix-icon">
</slot>
<div id="hoverBackground" part="hoverBackground"></div></template>
    <!--?lit$616380449$-->Restore default shortcuts
  </cr-button>
</cr-toast-manager>
<!--_html_template_end_--></template>
          </cr-most-visited>
        
        <!--?lit$616380449$-->
          <ntp-modules id="modules" modules-shown-to-user="" style="--container-gap: 8px; --container-max-width: 861px;"><template shadowrootmode="open"><!----><!--_html_template_start_--><div id="container">
  <!--?lit$616380449$--><!---->
    <ntp-module-wrapper><template shadowrootmode="open"><!----><!--_html_template_start_--><div id="impressionProbe"></div>
<div id="moduleElement">
  <slot id="slot"></slot>
</div>
<!--_html_template_end_--></template>
    <!----><ntp-drive-module format="wide" style="width: 728px;"><template shadowrootmode="open"><!----><!--_html_template_start_--><ntp-module-header id="moduleHeader" header-text="Google Drive" more-actions-text="More actions for Google Drive"><template shadowrootmode="open"><!----><!--_html_template_start_--><div id="titleContainer">
  <h2 id="title"><!--?lit$616380449$-->Google Drive</h2>
  <div id="headerSpacer"></div>
  <slot name="title-actions"></slot>
  <cr-icon-button id="menuButton" class="icon-more-vert" title="More actions for Google Drive" role="button" tabindex="0" aria-disabled="false"><template shadowrootmode="open"><!---->
<div id="icon">
  <div id="maskedImage"></div>
</div></template>
  </cr-icon-button>
</div>

<cr-action-menu id="actionMenu" role-description="More actions"><template shadowrootmode="open"><!---->
<dialog id="dialog" part="dialog" role="application" aria-roledescription="More actions">
  <div id="wrapper" class="item-wrapper" role="menu" tabindex="-1">
    <slot id="contentNode"></slot>
  </div>
</dialog></template>
  <!--?lit$616380449$--><!---->
    <button class="dropdown-item" id="disable" data-action="disable" role="menuitem">
      <cr-icon class="action-menu-icon cr-icon" icon="modules:block"><template shadowrootmode="open"><svg id="baseSvg" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid meet" focusable="false" viewBox="0 0 20 20" class="cr-iconset-svg-icon_" style="display: block; height: 100%; width: 100%; pointer-events: none;">
<g>
        <path d="M6.895 17.375a8.068 8.068 0 0 1-2.551-1.719 8.068 8.068 0 0 1-1.719-2.55A7.78 7.78 0 0 1 2 10c0-1.11.207-2.148.625-3.113a8.122 8.122 0 0 1 1.719-2.543c.73-.73 1.578-1.301 2.55-1.719A7.81 7.81 0 0 1 10.013 2a7.72 7.72 0 0 1 3.101.625 8.122 8.122 0 0 1 2.543 1.719c.73.73 1.301 1.578 1.719 2.543A7.75 7.75 0 0 1 18 10a7.78 7.78 0 0 1-.625 3.105 8.068 8.068 0 0 1-1.719 2.551c-.73.73-1.578 1.301-2.543 1.719a7.72 7.72 0 0 1-3.101.625 7.81 7.81 0 0 1-3.117-.625ZM10 16.5c.766 0 1.484-.125 2.168-.375a6.545 6.545 0 0 0 1.852-1.043L4.918 5.98a6.545 6.545 0 0 0-1.043 1.852A6.246 6.246 0 0 0 3.5 10c0 1.805.633 3.34 1.895 4.605C6.66 15.867 8.195 16.5 10 16.5Zm5.082-2.48a6.545 6.545 0 0 0 1.043-1.852c.25-.684.375-1.402.375-2.168 0-1.805-.633-3.34-1.895-4.605C13.34 4.133 11.805 3.5 10 3.5c-.766 0-1.484.125-2.168.375-.68.25-1.297.598-1.852 1.043ZM10 10Zm0 0"></path>
      </g></svg><!----></template></cr-icon>
      <!--?lit$616380449$-->Don't show Drive
    </button>
  <!----><!---->
    <button class="dropdown-item" id="info" data-action="info" role="menuitem">
      <cr-icon class="action-menu-icon cr-icon" icon="modules:info"><template shadowrootmode="open"><svg id="baseSvg" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid meet" focusable="false" viewBox="0 0 20 20" class="cr-iconset-svg-icon_" style="display: block; height: 100%; width: 100%; pointer-events: none;">
<g>
        <path d="M10.531 13.785a.73.73 0 0 0 .219-.535v-3.5c0-.21-.07-.39-.215-.535A.713.713 0 0 0 10.004 9c-.211 0-.39.07-.535.215a.73.73 0 0 0-.219.535v3.5c0 .21.07.39.215.535.14.145.32.215.531.215.211 0 .39-.07.535-.215Zm0-6.5a.716.716 0 0 0 .219-.531c0-.211-.07-.39-.215-.535A.716.716 0 0 0 10.004 6c-.211 0-.39.07-.535.215a.716.716 0 0 0-.219.531c0 .211.07.39.215.535.14.145.32.219.531.219.211 0 .39-.07.535-.215ZM10.004 18a7.8 7.8 0 0 1-3.11-.625 8.068 8.068 0 0 1-2.55-1.719 8.068 8.068 0 0 1-1.719-2.55A7.804 7.804 0 0 1 2 9.991c0-1.105.207-2.14.625-3.105a8.122 8.122 0 0 1 1.719-2.543c.73-.73 1.578-1.301 2.55-1.719A7.804 7.804 0 0 1 10.009 2c1.105 0 2.14.207 3.105.625a8.122 8.122 0 0 1 2.543 1.719c.73.73 1.301 1.578 1.719 2.547.418.968.625 2.004.625 3.105a7.8 7.8 0 0 1-.625 3.11 8.068 8.068 0 0 1-1.719 2.55c-.73.73-1.578 1.301-2.547 1.719a7.753 7.753 0 0 1-3.105.625ZM10 16.5c1.805 0 3.34-.633 4.605-1.895C15.867 13.34 16.5 11.805 16.5 10c0-1.805-.633-3.34-1.895-4.605C13.34 4.133 11.805 3.5 10 3.5c-1.805 0-3.34.633-4.605 1.895C4.133 6.66 3.5 8.195 3.5 10c0 1.805.633 3.34 1.895 4.605C6.66 15.867 8.195 16.5 10 16.5Zm0-6.5Zm0 0"></path>
      </g></svg><!----></template></cr-icon>
      <!--?lit$616380449$-->About this card
    </button>
  <!---->
  <!--?lit$616380449$-->
    <hr id="actionMenuDivider">
    <button id="customize-module" class="dropdown-item" data-action="customize-module" role="menuitem">
      <cr-icon class="action-menu-icon cr-icon" icon="modules:tune"><template shadowrootmode="open"><svg id="baseSvg" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid meet" focusable="false" viewBox="0 0 20 20" class="cr-iconset-svg-icon_" style="display: block; height: 100%; width: 100%; pointer-events: none;">
<g>
        <path d="M9.719 16.785a.73.73 0 0 1-.219-.535v-3.5c0-.21.07-.39.215-.535a.713.713 0 0 1 .531-.215c.211 0 .39.07.535.215a.73.73 0 0 1 .219.535v1h5.246c.211 0 .39.07.535.215.145.14.219.32.219.531 0 .211-.07.39-.215.535a.73.73 0 0 1-.535.219H11v1c0 .21-.07.39-.215.535a.713.713 0 0 1-.531.215c-.211 0-.39-.07-.535-.215ZM3.75 15.25c-.21 0-.39-.07-.535-.215A.713.713 0 0 1 3 14.504c0-.211.07-.39.215-.535a.73.73 0 0 1 .535-.219h3.5c.21 0 .39.07.535.215.145.14.215.32.215.531 0 .211-.07.39-.215.535a.73.73 0 0 1-.535.219Zm2.469-2.965A.73.73 0 0 1 6 11.75v-1H3.754c-.211 0-.39-.07-.535-.215A.716.716 0 0 1 3 10.004c0-.211.07-.39.215-.535a.73.73 0 0 1 .535-.219H6v-1c0-.21.07-.39.215-.535a.713.713 0 0 1 .531-.215c.211 0 .39.07.535.215a.73.73 0 0 1 .219.535v3.5c0 .21-.07.39-.215.535a.713.713 0 0 1-.531.215c-.211 0-.39-.07-.535-.215ZM9.75 10.75c-.21 0-.39-.07-.535-.215A.713.713 0 0 1 9 10.004c0-.211.07-.39.215-.535a.73.73 0 0 1 .535-.219h6.5c.21 0 .39.07.535.215.145.14.215.32.215.531 0 .211-.07.39-.215.535a.73.73 0 0 1-.535.219Zm2.469-2.965A.73.73 0 0 1 12 7.25v-3.5c0-.21.07-.39.215-.535A.713.713 0 0 1 12.746 3c.211 0 .39.07.535.215a.73.73 0 0 1 .219.535v1h2.75c.21 0 .39.07.535.215.145.14.215.32.215.531 0 .211-.07.39-.215.535a.73.73 0 0 1-.535.219H13.5v1c0 .21-.07.39-.215.535a.713.713 0 0 1-.531.215c-.211 0-.39-.07-.535-.215ZM3.75 6.25c-.21 0-.39-.07-.535-.215A.713.713 0 0 1 3 5.504c0-.211.07-.39.215-.535a.73.73 0 0 1 .535-.219h6.5c.21 0 .39.07.535.215.145.14.215.32.215.531 0 .211-.07.39-.215.535a.73.73 0 0 1-.535.219Zm0 0"></path>
      </g></svg><!----></template></cr-icon>
      Customise cards
    </button>
  
</cr-action-menu>
<!--_html_template_end_--></template>
</ntp-module-header>
<ntp-file-suggestion id="fileSuggestion" module-name="Drive" see-more-text="See more" see-more-aria-label="See more in Google Drive" see-more-url="https://drive.google.com"><template shadowrootmode="open"><!----><!--_html_template_start_--><div id="files">
  <!--?lit$616380449$--><!---->
    <a class="file" href="https://drive.google.com/open?id=1Wzur7IiZrWf4WmFcBgNrWrT4ytw_ngMFUu7FTSu7UzM&amp;usp=chrome_ntp" data-index="0" title="Untitled document">
      <div id="hover-layer"></div>
      <div class="icon-container">
        <img is="cr-auto-img" class="file-icon" draggable="false" auto-src="https://drive-thirdparty.googleusercontent.com/32/type/application/vnd.google-apps.document" src="chrome://image?https://drive-thirdparty.googleusercontent.com/32/type/application/vnd.google-apps.document">
      </div>
      <div class="file-info">
        <div class="file-title"><!--?lit$616380449$-->Untitled document</div>
        <div class="file-description"><!--?lit$616380449$-->You opened today</div>
      </div>
    </a>
  <!----><!---->
    <a class="file" href="https://drive.google.com/open?id=1y9lMFjq2f92ZEZBDJkjKwT69lO5IQ5GmsT7M1AELlFE&amp;usp=chrome_ntp" data-index="1" title="lets hack omer ackter">
      <div id="hover-layer"></div>
      <div class="icon-container">
        <img is="cr-auto-img" class="file-icon" draggable="false" auto-src="https://drive-thirdparty.googleusercontent.com/32/type/application/vnd.google-apps.document" src="chrome://image?https://drive-thirdparty.googleusercontent.com/32/type/application/vnd.google-apps.document">
      </div>
      <div class="file-info">
        <div class="file-title"><!--?lit$616380449$-->lets hack omer ackter</div>
        <div class="file-description"><!--?lit$616380449$-->You opened in the past week</div>
      </div>
    </a>
  <!----><!---->
    <a class="file" href="https://drive.google.com/open?id=1iW2C_DMFTs-ixVScbOF9kWhGwGTX5hUcGNT07iT7rV8&amp;usp=chrome_ntp" data-index="2" title="Untitled document">
      <div id="hover-layer"></div>
      <div class="icon-container">
        <img is="cr-auto-img" class="file-icon" draggable="false" auto-src="https://drive-thirdparty.googleusercontent.com/32/type/application/vnd.google-apps.document" src="chrome://image?https://drive-thirdparty.googleusercontent.com/32/type/application/vnd.google-apps.document">
      </div>
      <div class="file-info">
        <div class="file-title"><!--?lit$616380449$-->Untitled document</div>
        <div class="file-description"><!--?lit$616380449$-->You modified in the past week</div>
      </div>
    </a>
  <!----><!---->
    <a class="file" href="https://drive.google.com/open?id=1cMrdQ_zu4Xu_-Mm-RT1g82HQuZ2WBJHQ&amp;usp=chrome_ntp" data-index="3" title="WIN_20261112_09_47_39_Pro.mp4">
      <div id="hover-layer"></div>
      <div class="icon-container">
        <img is="cr-auto-img" class="file-icon" draggable="false" auto-src="https://drive-thirdparty.googleusercontent.com/32/type/video/mp4" src="chrome://image?https://drive-thirdparty.googleusercontent.com/32/type/video/mp4">
      </div>
      <div class="file-info">
        <div class="file-title"><!--?lit$616380449$-->WIN_20261112_09_47_39_Pro.mp4</div>
        <div class="file-description"><!--?lit$616380449$-->You opened in the past week</div>
      </div>
    </a>
  <!----><!---->
    <a class="file" href="https://drive.google.com/open?id=1Keg6gncvGm6K0PD4Kb5iQ8NSeafYRjd4asdh21Q9T9E&amp;usp=chrome_ntp" data-index="4" title="Water Crisis Research Task">
      <div id="hover-layer"></div>
      <div class="icon-container">
        <img is="cr-auto-img" class="file-icon" draggable="false" auto-src="https://drive-thirdparty.googleusercontent.com/32/type/application/vnd.google-apps.document" src="chrome://image?https://drive-thirdparty.googleusercontent.com/32/type/application/vnd.google-apps.document">
      </div>
      <div class="file-info">
        <div class="file-title"><!--?lit$616380449$-->Water Crisis Research Task</div>
        <div class="file-description"><!--?lit$616380449$-->You opened in the past week</div>
      </div>
    </a>
  <!----><!---->
    <a class="file" href="https://drive.google.com/open?id=1LFF2N-15NzrifOOGp-cmGZuN5FUZFNyY_nC1Vj6kD44&amp;usp=chrome_ntp" data-index="5" title="Exhibition group 7">
      <div id="hover-layer"></div>
      <div class="icon-container">
        <img is="cr-auto-img" class="file-icon" draggable="false" auto-src="https://drive-thirdparty.googleusercontent.com/32/type/application/vnd.google-apps.document" src="chrome://image?https://drive-thirdparty.googleusercontent.com/32/type/application/vnd.google-apps.document">
      </div>
      <div class="file-info">
        <div class="file-title"><!--?lit$616380449$-->Exhibition group 7</div>
        <div class="file-description"><!--?lit$616380449$-->You opened in the past week</div>
      </div>
    </a>
  <!---->
  <!--?lit$616380449$-->
    <div id="seeMoreButtonContainer">
      <a href="https://drive.google.com" aria-label="See more in Google Drive">
        <!--?lit$616380449$-->See more
        <div id="hoverContainer"></div>
      </a>
    </div>
  
</div>
<!--_html_template_end_--></template>
</ntp-file-suggestion>
<!--?lit$616380449$-->
<!--_html_template_end_--></template></ntp-drive-module></ntp-module-wrapper>
  <!---->
</div>
<cr-toast id="undoToast" duration="10000"><template shadowrootmode="open"><!----><slot></slot></template>
  <div id="undoToastMessage"><!--?lit$616380449$--></div>
  <!--?lit$616380449$-->
</cr-toast>
<!--_html_template_end_--></template>
          </ntp-modules>
        
        <!--?lit$616380449$-->
          <cr-toast id="undoToast" duration="10000"><template shadowrootmode="open"><!----><slot></slot></template>
            <div id="undoToastMessage"><!--?lit$616380449$--></div>
            <cr-button id="undoButton" aria-label="Press ⌘Z to undo" role="button" tabindex="0" aria-disabled="false"><template shadowrootmode="open"><!---->
<div id="background"></div>
<slot id="prefixIcon" name="prefix-icon">
</slot>
<span id="content">
  <slot></slot>
</span>
<slot id="suffixIcon" name="suffix-icon">
</slot>
<div id="hoverBackground" part="hoverBackground"></div></template>
              Undo
            </cr-button>
          </cr-toast>
        
        <!--?lit$616380449$-->
      <!--?lit$616380449$-->
          <a id="backgroundImageAttribution" href="" hidden="">
            <div id="backgroundImageAttribution1Container">
              <div id="linkIcon" hidden=""></div>
              <div id="backgroundImageAttribution1">
                <!--?lit$616380449$-->
              </div>
            </div>
            <div id="backgroundImageAttribution2" hidden="">
              <!--?lit$616380449$-->
            </div>
          </a>
          <!--?lit$616380449$-->
            <ntp-customize-buttons id="customizeButtons" show-shadow="" show-background-image="" modules-shown-to-user=""><template shadowrootmode="open"><!----><!--_html_template_start_-->
<div id="customizeButtons">
  <!--?lit$616380449$-->
  <cr-button id="customizeButton" class="customize-button" title="Customise this page" aria-pressed="false" role="button" tabindex="0" aria-disabled="false" has-prefix-icon_=""><template shadowrootmode="open"><!---->
<div id="background"></div>
<slot id="prefixIcon" name="prefix-icon">
</slot>
<span id="content">
  <slot></slot>
</span>
<slot id="suffixIcon" name="suffix-icon">
</slot>
<div id="hoverBackground" part="hoverBackground"></div></template>
    <cr-icon class="customize-icon" slot="prefix-icon" icon="ntp:pencil-custom"><template shadowrootmode="open"><svg id="baseSvg" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid meet" focusable="false" viewBox="0 0 24 24" class="cr-iconset-svg-icon_" style="display: block; height: 100%; width: 100%; pointer-events: none;">
<g width="24" height="24">
        <path d="M3 17.25V21h3.75L17.81 9.94l-3.75-3.75L3 17.25zM20.71 7.04a.996.996 0 0 0 0-1.41l-2.34-2.34a.996.996 0 0 0-1.41 0l-1.83 1.83 3.75 3.75 1.83-1.83z"></path><path d="M0 0h24v24H0z" fill="none"></path>
      </g></svg><!----></template>
    </cr-icon>
    <div id="customizeText" class="customize-text" hidden="">
      Customise Chrome
    </div>
  </cr-button>
</div>
<!--_html_template_end_--></template>
            </ntp-customize-buttons>
          
        
        <!--?lit$616380449$-->
      
      <div id="contentBottomSpacer"></div>
      <!--?lit$616380449$-->
    </div>
  </div>
</div>
<!--?lit$616380449$-->
<!--?lit$616380449$-->
<svg width="0" height="0">
  <defs>
    <clipPath id="oneGoogleBarClipPath">
      <!-- Set an initial non-empty clip-path so the OneGoogleBar resize events
           are processed. When the clip-path is empty, it's possible for the
           OneGoogleBar to get into a state where it does not send  the
           'overlayUpdates' message which is used to populate this
           clip-path. -->
      
    <rect x="-8" y="-8" width="973" height="80"></rect></clipPath>
  </defs>
</svg>
<!--_html_template_end_--></template></ntp-app>
