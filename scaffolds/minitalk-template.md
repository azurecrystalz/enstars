<!---
ONE CHARACTER
--->

<div class="minitalk" character="Anzu">
  <div class="minitalk-option">
    <div class="minitalk-option_header tab-header__open"><i>Option 1</i></div>
      <div class="minitalk-option_content" style="display: none;">
        <div class="msr-unit" character="[CHARACTER NAME]">
          <div class="msr-icon">
            <div class="msr-icon__wrapper">
              <div class="msr-icon__base"></div>
            </div>
          </div>
          <div class="msr-name"></div>
          <div class="msr-line">
            <p>Response Line One</p>
            <p>Response Line Two</p>
          </div>
        </div>
      </div>
    </div>
    <div class="minitalk-option">
    <div class="minitalk-option_header tab-header__open"><i>Option 2</i></div>
      <div class="minitalk-option_content" style="display: none;">
        <div class="msr-unit" character="[CHARACTER NAME]" attribute="">
          <div class="msr-icon">
            <div class="msr-icon__wrapper">
              <div class="msr-icon__base"></div>
            </div>
          </div>
          <div class="msr-name"></div>
          <div class="msr-line">
            <p>Response Line One.</p>
            <p>Response Line Two.</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<!---
2+ CHARAS
--->

<div class="minitalk" character="Anzu">
  <div class="minitalk-option">
    <div class="minitalk-option_header tab-header__open"><i>Option 1</i></div>
      <div class="minitalk-option_content" style="display: none;">
        <div class="msr-unit" character="[CHARACTER 1 NAME]">
          <div class="msr-icon">
            <div class="msr-icon__wrapper">
              <div class="msr-icon__base"></div>
            </div>
          </div>
          <div class="msr-name"></div>
          <div class="msr-line">
            <p>Response Line 1</p>
          </div>
        </div>
        <div class="msr-unit" character="[CHARACTER 2 NAME]">
          <div class="msr-icon">
            <div class="msr-icon__wrapper">
              <div class="msr-icon__base"></div>
            </div>
          </div>
          <div class="msr-name"></div>
          <div class="msr-line">
            <p>Response Line 2</p>
          </div>
        </div>
      </div>
    </div>
    <div class="minitalk-option">
    <div class="minitalk-option_header tab-header__open"><i>Option 2</i></div>
      <div class="minitalk-option_content" style="display: none;">
        <div class="msr-unit" character="[CHARACTER 1 NAME]" attribute="">
          <div class="msr-icon">
            <div class="msr-icon__wrapper">
              <div class="msr-icon__base"></div>
            </div>
          </div>
          <div class="msr-name"></div>
          <div class="msr-line">
            <p>Response Line 1</p>
          </div>
        </div>
        <div class="msr-unit" character="[CHARACTER 2 NAME]" attribute="">
          <div class="msr-icon">
            <div class="msr-icon__wrapper">
              <div class="msr-icon__base"></div>
            </div>
          </div>
          <div class="msr-name"></div>
          <div class="msr-line">
            <p>Response Line 2</p>
          </div>
        </div>
      </div>
    </div>
  </div>

<!---
STORY MINITALKS, 4 OUTCOMES PER TALK

TEST THIS CODE LATER
--->

<div class="minitalk" character="Character">
    <div class="minitalk-option">
        <div class="minitalk-option_header">
            Option 1
        </div>
        <div class="minitalk-option_content ">
            <ul class="tabber">
                <li class="active"><a data-tab="1a-n">Normal</a></li>
                <li><a data-tab="1a-r">Rare</a></li>
            </ul>
            <div data-tab="1a-n"> <!--- NORMAL OPTION --->
                {% bubble Character %}
                    Text
                {% endbubble %}
            </div>
            <div data-tab="1a-r" style="display: none"> <!--- RARE OPTION --->
                {% bubble Character %}
                    Text
                {% endbubble %}
            </div>
        </div>
    </div>
    <div class="minitalk-option">
        <div class="minitalk-option_header">
            Option 2
        </div>
        <div class="minitalk-option_content ">
            <ul class="tabber">
                <li class="active"><a data-tab="1b-n">Normal</a></li>
                <li><a data-tab="1b-r">Rare</a></li>
            </ul>
            <div data-tab="1b-n"> <!--- NORMAL OPTION --->
                {% bubble Character %}
                    Text
                {% endbubble %}
            </div>
            <div data-tab="1b-r" style="display: none"> <!--- RARE OPTION --->
                {% bubble Character %}
                    Text
                {% endbubble %}
            </div>
        </div>
    </div>
</div>