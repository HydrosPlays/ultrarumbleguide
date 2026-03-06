<style>
    .image-container {
        flex-direction: row;
        padding: 15px;
    }

    
    .container-image-icon {
        flex: 1 1 auto;
        max-width: 100px;
        max-height: 150px;
        object-fit: contain;
    }

    .role-image {
        max-width: 35px;
        max-height: 35px;  
    }

    .role-heading {
        display: flex;
        font-weight: 700;
        align-items: center;
        gap: 8px;
    }

    .role-heading p {
        margin: 0;
        line-height: 1.2;
        display: flex;
        align-items: center;
    }

@media (max-width: 768px) {
        .container-image-icon {
            max-width: 75px; 
            max-height: 100px;
        }
        
        .image-container {
            gap: 5px;
            margin-bottom: 10px;
            padding: 7px;
        }
}

.container-image-icon {
    max-width: 100px !important;
}
</style>

<p align="center">
    <img style="border-radius: 15px;" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/guide-infopedia.jpg" width="100%"/>
</p>

# <a style="color: lime !important;">CHARACTER CONDITIONS</a><br>
In this sub-guide you'll learn about My Hero Ultra Rumble's Character Conditions!

## What's a Character Condition?

Character Conditions are effects/states that can be applied to characters, anything that gets applied to a character, such a Burn, Freeze, Deafen and Low Gravity, as well as more complex ones such as Hardening, Blueflame and Gearshift. In this page you will also learn about interesting and unexplored facts about these states, such as their relationship with the KO Assist stat.

You will notice that all conditions have a section called Condition Data. If you're wondering what each tag means, use your best guess, since the meaning of each of them isn't written anywhere, however here's what they could mean:

- Priority: Likely which one has the highest priority when it comes to rendering, so that players with many effects don't look like a colorful mass.
- NotUseResult: No idea, probably related to the result screen, or maybe it determines whether damage caused by this effect counts towards your damage count.
- AllyBuff: Specifies if this is an ally buff or not.
- EnemyDebuff: Specifies if this is an enemy debuff or not.
- The rest: No idea, but it seems either KoAssistTimeMargin or KoAssistEndConditionTimerMargin indicate for how long will the "this is your KO assist" linger for until it goes away and the kill no longer counts as your assist.

## Navigation
Click the effect you wish to learn about. Click the gray arrow button on the bottom right of the page to quickly scroll up.

<div class="image-container">
    <a href="https://ultrarumble.com/guide/character-conditions#poison_mist" target="_self"> <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/poison_condition.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/burn_condition.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/burnblue_condition.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/freeze_condition.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/decay_condition.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/infectiondecay_condition.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shock_condition.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/erasure_condition.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/decreasehealth_condition.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/recoverhealth_condition.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/continuousrecoverhealth_condition.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/influenceheal_condition.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/dying_condition.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/transform_condition.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/bloodholder_condition.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/guard_condition.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/levelup_condition.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/speeddown_condition.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/piggyback_condition.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/lowgravity_condition.png" />
</div>

# Character Conditions

## Poison

<p align="center">
    <a id="poison_mist">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_poison.png" width="380" />
</p>

Poison is the Poison Mist's signature effect. To most players this wouldn't even be considered a condition per se, but in the game files they are one. Poison damage increases with a match's phase, dealing more damage as the match progresses. The name of this condition in the files is "PoizonMist", get used to seeing typos in the variable names.

Condition Data:
- Internal Name: <a style="color: orange !important;">PoizonMist</a><br>
- Condition Number: <a style="color: orange !important;">0</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Burn

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_burn.png" width="280" />
</p>

Burn is the signature DoT status effect of fire-based skills. It envelops players with an orange outline, and deals True DMG with duration and damage defined by each skill. This effect does not go away when touching water, but it can be countered with the special tune Resist Heat, though this is useless, as getting rid of this effect is the least of your concerns due to its terribly low DMG. Burn's name in the files is "Burn".<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Burn</a><br>
- Condition Number: <a style="color: orange !important;">1</a><br>
- Priority: <a style="color: orange !important;">3000</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">15.0</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can apply Burn is as follows:

### Burn Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/todoroki_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/todoroki_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/armormight_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/endeavor_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/endeavor_assault.png" />
</div>

### Conditional Burn Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mirio_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mrcompress_support.png" />
</div>

## Freeze

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_freeze.png" width="280" />
</p>

Freeze is a state effect inflicted by dealing 100 Freezepower to the enemy. Freezepower is a hidden stat ice moves have that determines how much freeze they apply to the character. Characters that become frozen are unable to move for a very short amount of time, and can be attacked while in this state. Frozen characters will have a layer of ice covering their body temporarily. Some abilities don't apply 100 Freezepower, meaning you need to land them multiple times to freeze, such is the case of Strike Shoto's beta, melee 2, and Armored All Might's ice bullet. This state can be blocked by the Resist Freeze special tune, though due to only providing benefit over freeze skills it's never really used.<br>
Freeze's name in the files is "Freeze".<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Freeze</a><br>
- Condition Number: <a style="color: orange !important;">2</a><br>
- Priority: <a style="color: orange !important;">2200</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">15.0</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can apply Freeze is as follows:

### Freeze Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/todoroki_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/todoroki_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/armormight_technical.png" />
</div>

### Conditional Freeze Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mirio_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mrcompress_support.png" />
</div>

## Decay

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_decay.png" width="280" />
</p>

Decay is one of Tomura Shigaraki's signature conditions. Affected players will see their Defense reduced temporarily by the value dictated by the source (10% for Embrittlement, 20% for Collapse Hand). This condition can be visually identified by how the affected character has a glitchy purple overlay texture.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Decay</a><br>
- Condition Number: <a style="color: orange !important;">3</a><br>
- Priority: <a style="color: orange !important;">3000</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">15.0</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can apply Decay is as follows:

### Decay Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shigaraki_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shigaraki_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shigaraki_technical.png" />
</div>

### Conditional Decay Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Blue Burn

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_burnblue.png" width="280" />
</p>

Blue Burn is Dabi's signature DoT status effect. It envelops players with a blue outline, and deals True DMG with duration and damage defined by each skill. This effect does not go away when touching water, but it can be countered with the special tune Resist Heat, though this is useless, as getting rid of this effect is the least of your concerns due to its terribly low DMG.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">BlueFlame</a><br>
- Condition Number: <a style="color: orange !important;">4</a><br>
- Priority: <a style="color: orange !important;">3000</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">15.0</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can apply Blue Burn is as follows:

### Blue Burn Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/dabi_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/dabi_strike.png" />
</div>

### Conditional Blue Burn Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mirio_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mrcompress_support.png" />
</div>

## Shock

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_shock.png" width="280" />
</p>

Shock is a state effect inflicted by dealing 100 Shockpower to the enemy. Shockpower is a hidden stat Denki Kaminari's moves have that determines how much freeze they apply to the character. Characters that become shocked are stunned for a relatively short amount of time, and can be attacked while in this state. Shocked characters will have subtle electric particles around them, and will often do funny noises. Some abilities don't apply 100 Shockpower, meaning you need to land them multiple times to shock, such is the case of both Kaminari's alpha skills. This status can be blocked by the special tune Resist Shock, but it's usually considered useless as it's only useful against Denki Kaminari's skills, so it's use is mostly reserved to blocking the special tune "Electrification", but even then any other tune will be more useful.<br>
Shock's name in the files is "Tunder", which is supposed to say Thunder but the code is full of typos like this...<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Tunder</a><br>
- Condition Number: <a style="color: orange !important;">5</a><br>
- Priority: <a style="color: orange !important;">3000</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">15.0</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can apply Shock is as follows:

### Shock Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/kaminari_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/kaminari_technical.png" />
</div>

### Conditional Shock Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mirio_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mrcompress_support.png" />
</div>

## Erasure

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_erasure.png" width="230" />
</p>

Erasure is Shota Aizawa's signature condition, which seals the use of the affected character's main 3 abilities (Alpha, Beta and Gamma). The name of this condition in the files is "UniqueSeal".<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">UniqueSeal</a><br>
- Condition Number: <a style="color: orange !important;">6</a><br>
- Priority: <a style="color: orange !important;">2500</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">15.0</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">20.0</a><br>

The distribution of characters that can apply Erasure is as follows:

### Erasure Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/aizawa_technical.png" />
</div>

### Conditional Erasure Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Decrease Health

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_decreasehealth.png" width="280" />
</p>

Unknown as to where exactly this is used, but judging by the name, this should decrease the player's health, likely instantaneously.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">DecreaseHealth</a><br>
- Condition Number: <a style="color: orange !important;">7</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Recover Health

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_recoverhealth.png" width="280" />
</p>

Unknown as to where exactly this is used, but judging by the name, this should recover the player's health, likely instantaneously. Might be what recovery items use.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">RecoverHealth</a><br>
- Condition Number: <a style="color: orange !important;">8</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Continuous Recover Health

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_continuousrecoverhealth.png" width="280" />
</p>

Unknown as to where exactly this is used, but judging by the name, this should recover the player's health continuously. Might be related to Support Ability Cards, which have their dedicated condition further below, but this might be added on top. Support Nejire has a variation of this condition on her beta skill.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Continuous_Recover_Health, Ch025_Continuous_Recover_Health</a><br>
- Condition Number: <a style="color: orange !important;">9, 89</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: lime !important;">true</a>, <a style="color: red !important;">false</a><<br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Influence of Ally Ability Heal

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_influenceheal.png" width="280" />
</p>

Unknown as to where exactly this is used, but it likely is related to Support Ability Cards, specifically the area that heals allies around, as the name says Influence (the healing area) of ally (it's for allies) of ability heal (the word "ability" is only used to refer to Ability Cards, as quirk abilities are called "skills").<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">InfluenceOfAllyAbilityHeal</a><br>
- Condition Number: <a style="color: orange !important;">10</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Down

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_dying.png" width="280" />
</p>

The condition that refers to the DOWN state, in which your movement is highly impaired, you're unable to use items or abilities (except for Dabi's Special Action), and rely on DOWN HP to support your existence.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Dying</a><br>
- Condition Number: <a style="color: orange !important;">11</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Transform

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_transform.png" width="280" />
</p>

Transform is one of Himiko Toga's signature conditions. Transform allows the user to play as a different character in the battlefield, mimicking the levels of whoever you turn into and losing the ability to collect blood. This condition can be visually identified by the ability of seeing a teammate with their classic white outline, but with an arrow on top of their head instead of their name (don't mistake them by your allies though) Internally, this condition is referred to as "Transform".<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Transform</a><br>
- Condition Number: <a style="color: orange !important;">12</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters who can Transform is as follows:

### Transform Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Guard

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_guard.png" width="280" />
</p>

Unknown as to where exactly this is used, but judging by the name, this is probably related to GP (Guard Points), whether this condition is always active on players with GP, or only when getting hit and triggering the blocking animation is unknown.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Guard</a><br>
- Condition Number: <a style="color: orange !important;">13</a><br>
- Priority: <a style="color: orange !important;">1000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Quirk Level Up

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_levelup.png" width="280" />
</p>

Likely a condition triggered everytime the player levels up, it might be the reason why you briefly get a rainbow-ish aura when leveling up.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Unique_Level_Up</a><br>
- Condition Number: <a style="color: orange !important;">14</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Speed Down

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_speeddown.png" width="280" />
</p>

Unknown as to where exactly this is used, and it's unlikely to be Iida's burnout as there's another condition called "Skill_SpeedDown", along with "Skill_SpeedUp", while this one is just "SpeedDown".<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Speed_Down</a><br>
- Condition Number: <a style="color: orange !important;">15</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Piggyback

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_piggyback.png" width="280" />
</p>

A condition applied when using a Piggyback special action. This likely controls everything related to piggyback, mostly the defense buff and the speed buff, Internally, this is actually 4 conditions, one for Izuku Midoriya, one for Tenya Iida, another for All Might, and a generic PiggyBack condition.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_PiggyBack, Skill_PiggyBack_Ch001, Skill_PiggyBack_Ch005, Skill_PiggyBack_Ch012</a><br>
- Condition Number: <a style="color: orange !important;">16, 17, 18 and 24</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

### Piggyback Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/deku_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/deku_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/iida_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/allmight_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/allmight_rapid.png" />
</div>

### Conditional Piggyback Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Low Gravity

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_lowgravity.png" width="280" />
</p>

Low Gravity is Ochako Uraraka's signature effect. Players with this effect will jump higher and fall slower, and their momentum will be extended. This effect can be visually identified by a pinkish outline on the affected character. The name of this effect in the files is "LowGravity".<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_LowGravity</a><br>
- Condition Number: <a style="color: orange !important;">19</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

<br>
The distribution of characters that can use Low Gravity are as follows::

### Low Gravity Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/uraraka_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/uraraka_assault.png" />
</div>

### Conditional Low Gravity Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Recipro Boost

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_reciproboost.png" width="280" />
</p>

Recipro Boost is Iida's signature condition, which can be triggered through his gamma skill and allows him to run and attack extremely fast.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_SpeedUp</a><br>
- Condition Number: <a style="color: orange !important;">20</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can use Recipro Boost is as follows:

### Recipro Boost Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/iida_rapid.png" />
</div>

### Conditional Recipro Boost Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Recipro Out

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_reciproout.png" width="280" />
</p>

Recipro Out is Iida's other signature condition, which triggers when his gamma skill runs out, greatly reducing his movement and attack speed and disabling the use of skills.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_SpeedDown</a><br>
- Condition Number: <a style="color: orange !important;">21</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can suffer Recipro Out is as follows:

### Recipro Out Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/iida_rapid.png" />
</div>

### Conditional Recipro Out Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Dumb

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_dumb.png" width="280" />
</p>

Dumb is a self-inflicting condition unique to Strike Denki Kaminari's beta skill. When this effect is active, the player will be able to walk around with reduced speed, but won't be able to attack or jump..<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_Aho</a><br>
- Condition Number: <a style="color: orange !important;">22</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Hardening

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_hardening.png" width="280" />
</p>

Hardening is Eijiro Kirishima's signature condition, which grants 40% Defense and superarmor, making the character resistant to flinching. This condition can be identified visually by a spiky red-orange aura around the character..<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_Unbreakable</a><br>
- Condition Number: <a style="color: orange !important;">23</a><br>
- Priority: <a style="color: orange !important;">2050</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Giant

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_giant.png" width="280" />
</p>

Giant is Mt Lady's signature condition, which allows the player to become gigantic, granting 70% Defense and superarmor, as well as altering their speed and jump..<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_Giant</a><br>
- Condition Number: <a style="color: orange !important;">25</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Infection Decay

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_infectiondecay.png" width="280" />
</p>

Infection Decay is the signature DoT status effect of Tomura Shigaraki. It envelops players with a red shattered air aura, and deals True DMG with duration and damage defined by each skill. This effect has the particular property of spreading to enemies that are close enough to the affected player, spreading around like a virus. Infection Decay's name in the files is "InfectionDecay".<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">InfectionDecay_Before, InfectionDecay_After, InfectionDecay_Sorce</a><br>
- Condition Number: <a style="color: orange !important;">0</a><br>
- Priority: <a style="color: orange !important;">3000</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">15.0</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can apply Infection Decay is as follows:

### Infection Decay Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shigaraki_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shigaraki_technical.png" />
</div>

### Conditional Infection Decay Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mirio_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/allmight_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mrcompress_support.png" />
</div>

## Strike Boost

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_strikeboost.png" width="280" />
</p>

Strike Boost is the condition given by the activation of a Strike Ability Card, increasing your damage output.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Ability_Attack</a><br>
- Condition Number: <a style="color: orange !important;">28</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Assault Boost

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_assaultboost.png" width="280" />
</p>

Assault Boost is the condition given by the activation of an Assault Ability Card, increasing your defense.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Ability_Durable</a><br>
- Condition Number: <a style="color: orange !important;">29</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Rapid Boost

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_rapidboost.png" width="280" />
</p>

Rapid Boost is the condition given by the activation of a Rapid Ability Card, increasing your movement and attack speed, and giving you the ability to Wall Run. On some moves like Assault Kirishima's alpha or Technical Mirio's beta, it can actually increase the amount of hits from the move, which leads to a higher damage output (a common trait in abilities that increase attack speed). The damage increase is lower than that of a Strike Card however.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Ability_MoveSpeed</a><br>
- Condition Number: <a style="color: orange !important;">30</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Support Boost

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_supportboost.png" width="280" />
</p>

Support Boost is the condition given by the activation of a Support Ability Card, granting you a healing aura that heals yourself and your allies, though it's likely that not this whole ability belongs to Support Boost, and instead part of it comes from the Influence of Ally Ability Heal condition.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Ability_Heal</a><br>
- Condition Number: <a style="color: orange !important;">31</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Technical Boost

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_technicalboost.png" width="280" />
</p>

Technical Boost is the condition given by the activation of a Technical Ability Card, increasing your reloading speed.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Ability_Technique</a><br>
- Condition Number: <a style="color: orange !important;">32</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Superarmor

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_superarmor.png" width="280" />
</p>

Superarmor is a special state granted temporarily by armored moves. This state prevents the player from flinching or be easily blown away, allowing them to fight back even while receiving an attack that normally wouldn't let them counterattack. This effect is visually represented through a yellow outline covering the player. Internally, there are 3 superarmor conditions, these being For Attack, For Damage and For Plus Ultra.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">SuperArmor_For_Attack, SuperArmor_For_Damage, SuperArmor_For_Plus</a><br>
- Condition Number: <a style="color: orange !important;">33, 34 and 35</a><br>
- Priority: <a style="color: orange !important;">2000, 0 and 2201</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>
<br>
The distribution of characters that possess at least 1 armored instance is as follows:

### Superarmor Characters
Characters that at least can use 1 ability with at least 1 instance of Superarmor.
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/deku_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/dekuofa_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/iida_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/kirishima_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/kirishima_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/kendo_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/kendo_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/ibara_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/tamaki_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/allmight_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/allmight_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/endeavor_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/hawks_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mtlady_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shigaraki_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shigaraki_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/yafo_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/dabi_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mrcompress_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/kurogiri_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/overhaul_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/overhaul_assault.png" />
</div>

### Conditional Superarmor Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Plus Ultra

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_plusultra.png" width="280" />
</p>

Plus Ultra is a special condition achieved by reaching 100% Plus Ultra meter and triggering it. Plus Ultra is a state that lasts for 15s by default and grants faster reload speed and level 9 skills (with a 20% DMG boost) temporarily, and restores all of the user's GP. Plus Ultra does not provide a defense or mobility buff.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">PlusUltra</a><br>
- Condition Number: <a style="color: orange !important;">36</a><br>
- Priority: <a style="color: orange !important;">2200</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Invincibility

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_invincible.png" width="280" />
</p>

The Invincibility condition makes the player immune to any source of damage, be it from attacks, DoTs, or the Poison Mist. This condition is given after being knocked down via 500 Downpower. This condition can be visually identified by characters glowing white.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Show_Invincible</a><br>
- Condition Number: <a style="color: orange !important;">37</a><br>
- Priority: <a style="color: orange !important;">12000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Compression 

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_compression.png" width="280" />
</p>

Compression is one of Mr. Compress' signature conditions. Currently unknown as to which part of his compression this refers, whether the state of being compressed, or the one of carrying a compressed ally.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Compressition</a><br>
- Condition Number: <a style="color: orange !important;">38</a><br>
- Priority: <a style="color: orange !important;">9000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can compress is as follows:

### Compression Characters
Characters that can compress.
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mrcompress_support.png" />
</div>

### Conditional Compression Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Compression Regeneration

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_compressionregen.png" width="280" />
</p>

Compression Regeneration is Mr. Compress's other signature condition, which heals affected characters over time. This effect can be applied via Mr. Compress's special action.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Compressition_Regeneration</a><br>
- Condition Number: <a style="color: orange !important;">39</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can apply compression regeneration is as follows:

### Compression Regeneration Characters
Characters that can apply compression regeneration.
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mrcompress_support.png" />
</div>

### Conditional Compression Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Camouflage

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_camouflage.png" width="280" />
</p>

Camouflage is a special state some characters can apply to themselves, which renders them nearly invisible, only really able to see the character's edges. This state actually has some cool benefits to eat, such as being untrackable by tracking mark moves like Denki Kaminari's alpha or Izuku Midoriya OFA's overdrive gamma (if activated before their attack started), it also hides the Mark effect, serving as a counter of this effect. It also grants the character a speed boost.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Opticaldazzlepaint</a><br>
- Condition Number: <a style="color: orange !important;">40</a><br>
- Priority: <a style="color: orange !important;">10000</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can use Camouflage are as follows::

### Camouflage Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/froppy_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/tamaki_strike.png" />
</div>

### Conditional Camouflage Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Permeation

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_permeation.png" width="280" />
</p>

Permeation is Mirio Togata's signature state, which allows the user to be immune to damage or ability effects and walk through walls, floors, ceilings and other obstacles, with some exceptions. This effect can be visually identified by a blue/cyan outline and blue particles emanating from the user's body, as well as a shiny noise.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_Transparent_Ch024</a><br>
- Condition Number: <a style="color: orange !important;">41</a><br>
- Priority: <a style="color: orange !important;">15000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can use permeation are as follows::

### Permeation Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mirio_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mirio_technical.png" />
</div>

### Conditional Permeation Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Display Health On Hit

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_displayhp.png" width="280" />
</p>

This is an unknown condition that, judging by the name, displays the enemy's HP upon receivign a hit. Internally, it's marked as being NEITHER an Ally Buff nor an Enemy Debuff. It's unclear if this condition is what's used for Technical Shigaraki's alpha Search, partly due to the fact that conditions are roughly ordered by when they were introduced, so if we guide ourselves by that, this should have been introduced between Season 5 and Season 7.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Disp_Health_On_Hit</a><br>
- Condition Number: <a style="color: orange !important;">42</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Display Guardpoint On Hit

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_displaygp.png" width="280" />
</p>

This is an unknown condition that, judging by the name, displays the enemy's GP upon receivign a hit. Internally, it's marked as being NEITHER an Ally Buff nor an Enemy Debuff. It's unclear if this condition is what's used for Technical Shigaraki's alpha Search, partly due to the fact that conditions are roughly ordered by when they were introduced, so if we guide ourselves by that, this should have been introduced between Season 5 and Season 7.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Disp_Guardpoint_On_Hit</a><br>
- Condition Number: <a style="color: orange !important;">43</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Marked

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_marked.png" width="280" />
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_marked_demo.png" width="280" />
</p>

Marked is a special effect that makes the player visible through walls for the user who inflicted this effect and their team. Visually, this effect looks like a red outline, but behind a solid surface, it looks like a red silouhette. This effect does no damage, but can be helpful to locate enemies. This effect can be inflicted by a few skills and the special tune Perception. It is unknown if Disp_Location_On_Hit is the condition linked to this effect.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Disp_Location_On_Hit (?)</a><br>
- Condition Number: <a style="color: orange !important;">44 (?)</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>
<br>
The distribution of characters that can mark enemies are as follows::

### Marking Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/kaminari_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/hawks_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/hawks_strike.png" />
</div>

### Conditional Marking Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mirio_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/allmight_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mrcompress_support.png" />
</div>

## Orb Penalty

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_orbpenalty.png" width="280" />
</p>

Orb Penalty is an interesting but unknown condition that might be related to a seemingly discarded gamemode leaked back in Season 1 known as "Orb Battle", a gamemode where you likely had to collect as many orbs as possible spread across the map. Orb Penalty could be a condition applied to players with many orbs to slow them down and balance the leading positions, but this is pure speculation.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Orb_Penalty</a><br>
- Condition Number: <a style="color: orange !important;">45</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Leader

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_leader.png" width="280" />
</p>

The Leader state is a condition that is likely related to the seemingly discarded gamemode known as "Leaders Battle" (or previously, Kings Battle). This condition might have been given by default to each team's leader, granting them currently unknown benefits/hindrances, but likely made the player's death give more points to the enemy.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">LEADER</a><br>
- Condition Number: <a style="color: orange !important;">46</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Bloodholder

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_bloodholder.png" width="280" />
</p>

Bloodholder is Himiko Toga's other signature condition. Bloodholder is the condition in which the player holds the blood of another player without using it yet. This condition can be visually identified by a pinkish aura around the character, though this aura is invisible to enemies. Internally, this condition's name is "TransformStocking"<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Transform_Stocking</a><br>
- Condition Number: <a style="color: orange !important;">47</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters who can be Bloodholders is as follows:

### Bloodholder Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Restoration

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_allyrestoration.png" width="280" />
</p>

Restoration is one of Overhaul's signature conditions, which allows for the healing of HP and GP, higher than that from its sister condition "RebuildMyself". This condition is applied by Overhaul's Special Action to allies only.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_Rebuild</a><br>
- Condition Number: <a style="color: orange !important;">48</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>
<br>
The distribution of characters that can restore allies are as follows::

### Restoration Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/overhaul_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/overhaul_assault.png" />
</div>

### Conditional Restoration Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Deafen 

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_deafen.png" width="280" />
</p>

Deafen is Present Mic's signature effect, which makes the target unable to hear anything but a strong ringing noise, losing any audible feedback, though this effect is useless against players who already play with volume off or heavely impaired by background noise/music. The name of this effect in the files "Noise".<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Noise</a><br>
- Condition Number: <a style="color: orange !important;">49</a><br>
- Priority: <a style="color: orange !important;">3000</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">15.0</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that inflict Deafen are as follows::

### Deafen Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mic_strike.png" />
</div>

### Conditional Deafen Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Zero Gravity

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_zerogravity.png" width="280" />
</p>

Zero Gravity is Ochako Uraraka's other signature effect. Enemies affected by this condition will slowly float upwards, unable to attack or perform any mobe. The name of this effect in the files is "LowGravityToEnemy".<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_LowGravityToEnemy</a><br>
- Condition Number: <a style="color: orange !important;">50</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">15.0</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can use Low Gravity are as follows::

### Zero Gravity Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/uraraka_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/uraraka_assault.png" />
</div>

### Conditional Zero Gravity Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Copy

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_copy.png" width="280" />
</p>

Copy is one of Neito Monoma's signature conditions, which allows the use of copied abilities instead of the default ones. You can identify this condition by the magenta outline around the character and the presence of greenish bits in abilities that enlarge body parts or use new ones, such as wings or enlarged fists. Visually, this condition is very similar to "Steal".<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Copy</a><br>
- Condition Number: <a style="color: orange !important;">51</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can use copied abilities is as follows::

### Copy Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
</div>

### Conditional Copy Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Copyholder

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_copyholder.png" width="280" />
</p>

Copy is another of Neito Monoma's signature conditions, which stores copied abilities that can be used through the condition above.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Copy_Stocking</a><br>
- Condition Number: <a style="color: orange !important;">52</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can store copied abilities is as follows::

### Copyholder Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
</div>

### Conditional Copyholder Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Duplicate

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_duplicate.png" width="280" />
</p>

A condition likely linked to Twice, but still not clear as to how. It's possible that this condition is applied to the clones themselves, limiting which skills they can use i nthe case of beta clones.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Duplicate</a><br>
- Condition Number: <a style="color: orange !important;">53</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can inflict Duplicate is as follows::

### Duplicate Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/twice_rapid.png" />
</div>

### Conditional Duplicate Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Rule of HP Regeneration

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_hprule.png" width="280" />
</p>

An unknown condition that is likely related to Training Mode's HP Regeneration setting.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">RULE_HP_REGENERATION</a><br>
- Condition Number: <a style="color: orange !important;">54</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Rule of GP Regeneration

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_gprule.png" width="280" />
</p>

An unknown condition that is likely related to Training Mode's GP Regeneration setting.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">RULE_GP_REGENERATION</a><br>
- Condition Number: <a style="color: orange !important;">55</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Rule of Respawning

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_respawnrule.png" width="280" />
</p>

An unknown condition that is likely related to Training Mode and Area Control Battle's respawn mechanic.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Rule_Respawned</a><br>
- Condition Number: <a style="color: orange !important;">56</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

## Crazy Torch

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_crazytorch.png" width="280" />
</p>

Crazy Torch is Strike Dabi's signature condition, increasing damage by +20% and granting a movement speed boost, as well as granting special benefits to Strike Dabi's alpha and beta skills even on copy characters. Whether the flame circles count as part of the skill or part of the condition is unknown.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">WearBlueFlame</a><br>
- Condition Number: <a style="color: orange !important;">57</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can go Crazy Torch is as follows::

### Crazy Torch Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/dabi_strike.png" />
</div>

### Conditional Crazy Torch Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Steal

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_steal.png" width="280" />
</p>

Steal is All For One's signature condition, allowing the use of stolen quirk skills. Visually, this condition gives the character a magenta outline and makes enlarged or foreign bodyparts have a green tint.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_Steal</a><br>
- Condition Number: <a style="color: orange !important;">58</a><br>
- Priority: <a style="color: orange !important;">1000</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can Steal is as follows::

### Steal Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
</div>

### Conditional Steal Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Teleport

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_teleport.png" width="280" />
</p>

Teleport is a condition possibly related to All For One's gamma skill, allowing the teleportation of targets. Currently unknown if this condition is also applied to Kurogiri and his portals.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Teleport</a><br>
- Condition Number: <a style="color: orange !important;">59</a><br>
- Priority: <a style="color: orange !important;">500</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">15.0</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can Teleport enemies is as follows::

### Teleport Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
</div>

### Conditional Teleport Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Self-Restoration

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_restoration.png" width="280" />
</p>

Self-Restoration is another of Overhaul's signature conditions, which allows the instant restoration of all HP and some GP. This condition can be seen when using Overhaul's special action on yourself.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_RebuildMyself</a><br>
- Condition Number: <a style="color: orange !important;">60</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can use self-restoration is as follows::

### Self-Restoration Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/overhaul_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/overhaul_support.png" />
</div>

### Conditional Teleport Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Petrify

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_petrify.png" width="280" />
</p>

Petrify is Overhaul's signature state effect, inflicted by the skills Coffin of Absolute Shackles and Coffin Shot. Characters that become petrified are unable to move for a very short amount of time, and can be attacked while in this state. Petrified characters will have a layer of earth covering their body temporarily. This condition is actually 2 conditions, one is used by Support Overhaul's gamma, while the other is used by Assault's.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">StoneBind, StoneBindV2</a><br>
- Condition Number: <a style="color: orange !important;">61. 90</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">15.0</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>
<br>
The distribution of characters that can apply Petrify is as follows:

### Petrify Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/overhaul_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/overhaul_assault.png" />
</div>

### Conditional Petrify Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Tuning Conditions

Tuning often reuses conditions for its tuning effects, though in most cases this is technically done through a different condition that mimics most of the original condition while allowing it to work as a tuning skill, this is why technically the tuning Embrittlement does not apply "Decay" but instead applies "RollSlot_Decay", so if you notice strange differences between the conditions applied by tuning and the original ones, this is why. These are the conditions tied to tuning:

- RollSlot_Ability_Attack: <a style="color: orange !important;">62</a><br>
- RollSlot_Ability_Durable: <a style="color: orange !important;">63</a><br>
- RollSlot_Ability_MoveSpeed: <a style="color: orange !important;">64</a><br>
- RollSlot_Ability_Heal: <a style="color: orange !important;">65</a><br>
- RollSlot_Ability_Technical: <a style="color: orange !important;">66</a><br>
- RollSlot_Opticaldazzlepaint: <a style="color: orange !important;">67</a><br>
- RollSlot_Influence_Of_Ally_Ability_Heal: <a style="color: orange !important;">68</a><br>
- SuperArmor_For_RollSlot: <a style="color: orange !important;">69</a><br>
- RollSlot_Invincible: <a style="color: orange !important;">70</a><br>
- RollSlot_WallDash: <a style="color: orange !important;">71</a><br>
- RollSlot_SPAction_ReloadSpeed_Accel: <a style="color: orange !important;">72</a><br>
- RollSlot_Decay: <a style="color: orange !important;">75</a><br>
- RollSlot_Opticaldazzlepaint: <a style="color: orange !important;">79</a><br>
- RollSlot_Acceleration: <a style="color: orange !important;">82</a><br>
- RollSlot_Ability_Ch015_RECOVERY_HEALTH_GUARDPOINT: <a style="color: orange !important;">88</a><br>

## Brainwash

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_confusion.png" width="280" />
</p>

Brainwash is Hitoshi Shinso's signature condition, which decreases movement and attack speed greatly, fogs vision and hides teammates' overhead UI for the affected user. The only benefit for brainwashed enemy is that this effect also increases downpower received by 3, making it easier for the victim to be knocked down so they aren't comboed to death with ease. This effect can be visually identified by the moving question marks above the affected player.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_Brainwash_SpeedDown</a><br>
- Condition Number: <a style="color: orange !important;">73</a><br>
- Priority: <a style="color: orange !important;">1500</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">15.0</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>
<br>
The distribution of characters that can brainwash enemies are as follows::

### Brainwash Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shinso_strike.png" />
</div>

### Conditional Brainwash Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Special Brainwash

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_specialconfusion.png" width="280" />
</p>

Brainwash is Hitoshi Shinso's other signature condition, which takes away control from the enemy, not allowing them to do anything besides emoting, and can be directed somewhere else via Persona Command (Shinso's other Special Action). Taking any form of damage, even if it's Poison Mist damage, will dispel this effect. You can identify this condition by stars rotating above the affected character's head.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_Brainwash_Special</a><br>
- Condition Number: <a style="color: orange !important;">74</a><br>
- Priority: <a style="color: orange !important;">2000</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">15.0</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can cause special brainwash to enemies are as follows::

### Special Brainwash Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shinso_strike.png" />
</div>

### Conditional Special Brainwash Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Electrified

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_electrified.png" width="280" />
</p>

Electrified is one of Denki Kaminari's signature conditions. It allows to envelop one's body in electricity, briefly inflicting Shock and 150 Downpower when an enemy comes in contact with the electric aura.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_Special_Ch007</a><br>
- Condition Number: <a style="color: orange !important;">76</a><br>
- Priority: <a style="color: orange !important;">2200</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can electrify themselves are as follows::

### Electrified Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/kaminari_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/kaminari_technical.png" />
</div>

### Conditional Electrified Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Furious Ascent Armor

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_furiousascentarmor.png" width="280" />
</p>

Furious Ascent Armor is Strike Itsuka Kendo's signature condition, which grants the user high defense and superarmor, as well as blocking physical grabs such as Strike Dabi's.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_Ch046_Armor</a><br>
- Condition Number: <a style="color: orange !important;">77</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>
<br>
The distribution of characters that can use Furious Ascent Armor are as follows::

### Furious Ascent Armor Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/kendo_strike.png" />
</div>

### Conditional Furious Ascent Armor Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Steel 

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_steel.png" width="280" />
</p>

Steel is one of Neito Monoma's signature conditions, which protects the user from a single instance of damage and grants i-frames after.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_Ch104_Steel</a><br>
- Condition Number: <a style="color: orange !important;">78</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>
<br>
The distribution of characters that can go Steel are as follows::

### Steel Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
</div>

### Conditional Steel Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Transmission

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_transmission.png" width="280" />
</p>

Transmission is one of Izuku Midoriya OFA's signature conditions, which grants a speed boost that increases with the transmission level. At maximum transition level, it unlocks the full potential of Izuku Midoriya OFA's beta and gamma skills. This condition isn't the same as that of the tuning Acceleration, as this tuning has no ties with the overdrive system. This condition can be identified easily by the blue trails behind the character.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_Ch202_TransMission</a><br>
- Condition Number: <a style="color: orange !important;">80</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>
<br>
The distribution of characters that can use Transmission is as follows::

### Transmission Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/dekuofa_rapid.png" />
</div>

### Conditional Transmission Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Fa Jin

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_fajin.png" width="280" />
</p>

Fa Jin is Izuku Midoriya OFA's other signature condition, which increases horizontal and vertical jump height, allowing for high jumps and fast long jumps. This effect can be visually identified by the presence of reddish energy in the character's lower leg.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_Ch202_Hakkei</a><br>
- Condition Number: <a style="color: orange !important;">81</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>
<br>
The distribution of characters that can use Fa Jin is as follows::

### Fa Jin Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/dekuofa_rapid.png" />
</div>

### Conditional Fa Jin Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Special Action Seal

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_specialactionseal.png" width="280" />
</p>

Special Action Seal is All For One -Youth Age-'s signature condition, allowing to disable the use of the affected character's special action. You can visually identify this condition by the presence of black and red electricity around them.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">SpecialSeal</a><br>
- Condition Number: <a style="color: orange !important;">83</a><br>
- Priority: <a style="color: orange !important;">2099</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">15.0</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>
<br>
The distribution of characters that can seal special actions is as follows::

### Special Action Seal Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/yafo_assault.png" />
</div>

### Conditional Special Action Seal Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Perfect Permeation

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_perfectpermeation.png" width="280" />
</p>

Perfect Permeation is another of Mirio Togata's signature condition. This allows the user to permeate through any surface, literally any, from buildings that normally can't be permeated through, to the ground itself. This condition is used by Mirio's dash special action, and can sometimes lead to the character falling below the world (though underground there are "deathplanes" that teleport you back to the surface after hitting them).<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Skill_PerfectTransparent_Ch024</a><br>
- Condition Number: <a style="color: orange !important;">84</a><br>
- Priority: <a style="color: orange !important;">15000</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can use Perfect Permeation are as follows::

### Perfect Permeation Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mirio_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mirio_technical.png" />
</div>

### Conditional Perfect Permeation Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Super Recovery

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_superrecovery.png" width="280" />
</p>

Super Recovery is Technical Tomura Shigaraki's signature condition, which heals the character's HP and GP and inflicts Infection Decay to enemies near the Super Recovery player. This condition can be visually identified by the presence of red, black and purple particles emanating for the player's body.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Ch015_RECOVERY_HEALTH_GUARDPOINT</a><br>
- Condition Number: <a style="color: orange !important;">85</a><br>
- Priority: <a style="color: orange !important;">98</a><br>
- NotUseResult: <a style="color: lime !important;">true</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can use Super Recovery are as follows::

### Super Recovery Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shigaraki_technical.png" />
</div>

### Conditional Super Recovery Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Wave Veil

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_waveveil.png" width="280" />
</p>

Wave Veil is Support Nejire Hado's signature condition, which grants a veil that buffs Rapid Mirio Togata's beta, Technical Mirio Togata's gamma, Tamaki Amajiki's gamma, and Support Nejire Hado's alpha and beta skills. It's unknown if the Stamina points her gamma gives are part of the condition or just something her skill adds on top.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">CH025_WAVE_BARRIER</a><br>
- Condition Number: <a style="color: orange !important;">86</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: lime !important;">true</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: <a style="color: orange !important;">ECharacterConditionEndType::DESTRUCTION</a><br>
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can grant Wave Veil are as follows::

### Wave Veil Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/nejire_support.png" />
</div>

### Conditional Wave Veil Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Black Ankh

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_blackankh.png" width="280" />
</p>

Black Ankh is Fumikahe Tokoyami's signature condition, which enhances the user's melee capabilities, including damage, range, lunge, and the presence of projectiles emerging from melees. Black Ankh also boosts the upwards flight boost from Fumikage Tokoyami's flight special action.<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">Ch011_AbyssDarkBody</a><br>
- Condition Number: <a style="color: orange !important;">87</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -<br>
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can use Black Ankh are as follows::

### Black Ankh Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/tokoyami_assault.png" />
</div>

### Conditional Black Ankh Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Grab

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_grab.png" width="280" />
</p>

Grab is a condition applied by certain skills that immobilize the player while simultaneously dragging them, either physically or from a distance. It's speculated that not every "grab skill" actually applies this condition, and only those where the enemy character is suspended and moving their feet quickly are the ones that count as actual grabs (as the rest such as Tamaki's alpha or Assault Deku's gamma would fall in a different category that isn't managed by a condition).<br>
<br>
Condition Data:
- Internal Name: <a style="color: orange !important;">grab</a><br>
- Condition Number: <a style="color: orange !important;">91</a><br>
- Priority: <a style="color: orange !important;">0</a><br>
- NotUseResult: <a style="color: red !important;">false</a><br>
- KoAssist: <a style="color: red !important;">false</a><br>
- KoAssistTimeMargin: <a style="color: orange !important;">-</a><br>
- KoAssistEndTypeList: -<br>
- KoAssistEndConditionTimerMargin: <a style="color: orange !important;">-</a><br>

The distribution of characters that can Grab are as follows::

### Grab Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/ibara_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shinso_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/allmight_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/aizawa_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/dabi_strike.png" />
</div>

### Conditional Grab Characters
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

## Sleep

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_sleep.png" width="280" />
</p>

Sleep is an unknown condition that was found in a previous recent season but is currently removed. Apparently, this condition is applied to allies, not to enemies, which is definitely interesting considering sleep effects are often a debuff in games.

## Double Impact

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_twinimpact.png" width="280" />
</p>

Double Impact is an unknown condition that was found in a previous recent season but is currently removed. This condition's name is similar to that of a quirk called "Twin Impact" from Class 1-B, which has made some people speculate about a Neito Monoma Alternative Battle Style.





