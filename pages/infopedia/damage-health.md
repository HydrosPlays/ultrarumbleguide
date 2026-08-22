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
<em style="font-size: 14px;">Last Update: August 20th 2026</em>

# <a style="color: lime !important;">DAMAGE, HEALTH, HEALING AND INTERACTIONS</a><br>
In this sub-guide you'll learn about My Hero Ultra Rumble's health types and how damage works, as well as healing and skill-to-character interactions!

# Health Types
## Health Points (HP)

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_hp.png" width="280" />
</p>

This is the healthtype you care the most for most of the match, as losing it means you will enter the DOWN state, a state where you will be vulnerable and easy to kill, for this reason you want to avoid losing it. HP is fortunately protected by another healthtype: GP, which will take damage in place of HP (in some cases, you might also have "Stamina" to protect you, another healthtype).<br>
<br>
While normally GP and Stamina protect your HP, there are certain attacks that bypass this rule, attacking HP directly and ignoring GP/Stamina (or also damaging them too). HP can also be directly attacked by Poison Mist damage and that from DoT (Damage Over Time) effects such as Burning, Blue Burning and Decay.<br>
<br>
Players on HP that lack any blue health (GP) will not get stunned by certain moves and instead will often either keep moving or be blown away, however, when they get stunned they remain stunned for longer than if they had GP, which means in most cases players on HP only are easier to be combo'd.
<br>
HP appears as a green bar in your interface, but when damaged it will appear as orange damage numbers for the attacker. You can heal HP through HP Recovery drinks, Support Ability Cards, some special tunes and certain abilities.<br>
<br>
The distribution of characters by HP is as follows (keep in mind T.U.N.I.N.G. can increase a character's Max HP):

### 400 HP - Tanky 
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/kirishima_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/kendo_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/ibara_support.png" />
</div>

### 350 HP - Above Standard
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/bakugo_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/uraraka_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/todoroki_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/todoroki_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/momo_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/kaminari_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/kaminari_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/kendo_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/tamaki_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/allmight_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/armormight_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/cementoss_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/endeavor_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/endeavor_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mtlady_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/star_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/dabi_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/dabi_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/overhaul_support.png" />
</div>

### 300 HP - Standard
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/deku_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/deku_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/bakugo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/uraraka_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/iida_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/kirishima_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/tokoyami_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mirio_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/nejire_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/nejire_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shinso_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/allmight_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/aizawa_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/aizawa_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mic_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mic_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/hawks_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mirko_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shigaraki_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shigaraki_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shigaraki_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/yafo_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/twice_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/twice_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mrcompress_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/kurogiri_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/gentle_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/overhaul_assault.png" />
</div>

### 250 HP - Frail
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/dekuofa_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/bakugo_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/froppy_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mirio_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/hawks_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/nagant_strike.png" />
</div>

### ??? HP - Unknown
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/froppy_strike.png" />
</div>

## Guard Points (GP)

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_gp.png" width="280" />
</p>

The 2nd main healthtype. Unlike HP, every character has the same amount of GP, that being 250 GP (this amount can be increased via T.U.N.I.N.G. however). The purpose of GP is to protect your HP in fights, as most attacks won't be able to lower your HP if you still have GP. When this healthtype is depleted, a Guardbreak will occur, which by default doesn't really do anything, but some tuning effects trigger on self or enemy guardbreak.<br>
<br>
GP cannot protect the player from Poison Mist, DoT or True DMG. GP is often seen as less valuable than HP, not only because of GP being unable to protect you from those DMG sources, but also because in most cases characters have more Max HP than Max GP. A false belief that exists among some is that GP comes with a small defense boost, but this is NOT true.<br>
<br>
Healing GP first can sometimes be useful. When a player is hit by an attack, their character will react differently on GP compared to HP. On GP, stuns from attacks are shorter, meaning they can fight back earlier, which is important when it comes to combos, as this reduced window to stun makes some combos impossible or very difficult on GP. However, there are also abilities that work better against GP, a classic case is Mr. Compress's alpha marble, which doesn't stun on HP but does stun on GP. Another reason why you might like to heal GP is to trigger a special tune's effect, as some trigger on guardbreak. For example, if you heal GP, and then you get attacked while trying to heal HP, you might trigger a healing or defensive tuning that could help you out. In some cases, you can also use GP to make the enemy thing you have high health even if you're not, as otherwise you might get more targeted since the enemy could think you're low on health.<br>
<br>
GP appears as a blue bar in your interface, and when damaged it will appear as blue damage numbers for the attacker. GP can be recovered through GP Healing drinks, through some abilities and special tunes, and through activating Plus Ultra.<br>
<br>
If an attack breaks the player's guard, they'll be affected as if it were a hit on HP instead of GP, meaning the stun will be longer if it does happen. (These stun rules only apply to hitstun, not electric, freezing or grabbing stuns).

## DOWN Health Points (DOWN HP)

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_downhp.png" width="280" />
</p>

DOWN HP is the last thing protecting you from death. Once your HP reaches zero, you will be DOWNd, which will make you unable to use items or abilities (unless you're Dabi, who can use his Special Action), and your movement will be highly hindered. In this state, you will have 400 DOWN HP regardless of the character you're playing, and will be unable to be healed by healing items or abilities. As the player, there's little you can do to protect your DOWN HP beyond hiding, as this is mostly the responsibility of your teammates, and even then it's very difficult to protect a teammate long enough for them to get up on their own, so unless you're Dabi, have a character with revive abilities, or have a team that can defend you, you'll most likely die.<br>
<br>
DOWN HP appears as a red bar in your interface, replacing HP, and when damaged it will appear as dark red damage numbers for the attacker. DOWN HP can be increased via tuning, but it cannot be recovered. Getting up (either from a revive or by letting the DOWN timer hit zero) will reset your DOWN HP, so if you get DOWNd again you will have 400 DOWN HP again.

## Stamina

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/icon_stamina.png" width="280" />
</p>

Stamina (also known as Barrier Points internally) is a special type of health that can only be obtained through the skill "Spiraling Veil", which is Nejire Hado (Fairy)'s gamma skill. Stamina works like an "Overguard", protecting both your HP and GP (though attacks that bypass GP also bypass Stamina). For most things, Stamina works like a 2nd GP bar that you can see above your crosshair, and unlike HP or GP, this healthtype is temporary and cannot be healed back.<br>
<br>
Damaging a character with Stamina will show yellow damage numbers. DOWNd characters cannot receive Stamina

### Direct Sources of Stamina
Characters who have the ability to grant Stamina.<br>

<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/nejire_support.png" />
</div>

### Conditional Sources of Stamina
Characters who don't have the ability to grant Stamina by default, but can do it under certain circumstances (in this case, by copying or stealing Nejire's Spiraling Veil).

<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

# Damage

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/strikebig.png" width="180" />
</p>

Like in all games, damage is force that reduces a character's health by the values set in the code (decimal damage is rounded up, so 22.1 turns into 23 DMG). Damage can be amplified through Strike Ability Cards, some special tunes, some normal tunes, Plus Ultra, or/and by having teammates using Strike characters. You can also benefit from Defense DOWN debuffs to deal more damage to the affected target. Damage can be lower than expected when hitting enemies with Defense buffs, which can come from Assault Ability Cards, some special tunes, some normal tunes and/or having teammates using Assault characters. In the settings, you can configure how you want damage to show up, so if an enemy receives 20 DMG five times in quick succession, you can either configure it so shows as five 20s popping up, or as only 1 number getting bigger.<br>
<br>
There are various types of damage.

## Normal DMG

As the name implies, this is the most basic form of damage, damaging healthtypes in the following order: Stamina -> Guard Points -> Health Points.<br>
<br>

## True DMG

This is damage that bypasses Stamina and Guard Points, making it particularily lethal. True DMG can be inflicted via some abilities, DoT effects and the Poison Mist, which serves as extra incentive to heal HP. Poison Mist and DoT damage does not cause damage numbers to pop up, but True DMG abilities do.

### Characters with True DMG abilities.
Of this list, Ibara Shiozaki and Strike Tomura Shigaraki are the most dangerous, as at max level they can kill you in just 2 uses of their True DMG moves.

<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/deku_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/ibara_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shigaraki_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/nagant_strike.png" />
</div>

### Characters with DoT abilities.
Characters that can't deal True DMG directly but instead rely on DoTs, which cannot kill characters even if they are at 1 HP.

<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/todoroki_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/todoroki_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/endeavor_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/armormight_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/endeavor_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shigaraki_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shigaraki_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/dabi_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/dabi_strike.png" />
</div>

### Conditional True Damagers
Characters who don't have the ability to deal True DMG by default but can do so under certain circumstances.

<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mirio_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/allmight_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mrcompress_support.png" />
</div>

# Healing

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/supportbig.png" width="180" />
</p>

If damage reduces health, healing recovers it. Healing is mostly found in drinks and Support Ability Cards and Special Tunes, as actual healing abilities are extremely rare among the cast. Some abilities can heal HP, others can heal GP, and others heal both. While not the case for every healing ability, they often don't work inside the Poison Mist in an attempt to prevent camping. In most cases, the healing of abilities is set, and cannot be increased in any way, however Ibara Shiozaki's gamma allows her to heal the amount of damage she has dealt, so increased her gamma's damage will increase the healing she receives.

Being revived or getting up from the DOWN state gives you some HP back, but the HP you're given decreases with each time you get DOWNd. Revives can recover GP if the reviver has the Reinforced Revive tune, though this does not work on Dabi's special action.

### Healers
Characters with the ability to heal themselves and/or teammates (healing by reviving doesn't count). Of this list, Mr. Compress has the weakest and most limited healing, Overhaul has the greatest immediate healing, while Nejire has less healing power but is full of healing sources and gets more healing value than Overhaul fast. Honorable mention to Momo Yaoyorozu as she cannot heal allies directly, but can spawn Full Recovery Drinks which she can drink to heal allies.

<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/nejire_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/star_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/twice_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mrcompress_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/overhaul_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/overhaul_assault.png" />
</div>

### Self-Healers
Characters unable to heal allies and instead can only heal themselves (healing by reviving doesn't count).
<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/ibara_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/shigaraki_technical.png" />
</div>

### Conditional Healers
Characters who don't have the ability to heal by default but can do so under certain circumstances. Monoma's healing is lower due to his 80% effectiveness rule.

<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/monoma_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mirio_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/allmight_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/afo_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

### Heal Special Tunes
Special tunes with the ability to heal.

|    |  |
|----|--|
| <img src="https://ultrarumble.com/assets/roleslots/T_ui_UniqueSkill_ch012_01.png" width="125"> | **Muscle Form**<br>Heals the user's HP instantly after using PU.|
| <img src="https://ultrarumble.com/assets/roleslots/T_ui_UniqueSkill_ch101_00.png" width="125"> | **Revenge Support**<br>Heals the user and nearby allies' HP over time when the user's guard is broken.|
| <img src="https://ultrarumble.com/assets/roleslots/T_ui_UniqueSkill_ch015_02.png" width="125"> | **Hyper Regeneration** <br>Heals the user's HP and GP over time after breaking an enemy's guard.|
| <img src="https://ultrarumble.com/assets/roleslots/T_ui_UniqueSkill_ch018_00.png" width="125"> | **HP Sucker** <br>Heals the user's HP instantly upon DOWNing an enemy.|
| <img src="https://ultrarumble.com/assets/roleslots/T_ui_UniqueSkill_ch018_01.png" width="125"> | **GP Sucker** <br>Heals the user's GP instantly upon DOWNing an enemy.|
| <img src="https://ultrarumble.com/assets/roleslots/T_ui_UniqueSkill_ch034_00.png" width="125"> | **Reinforced Revive** <br>Teammates revived by the user of this tune are revived with GP.|

# Reviving

<p align="center">
    <img src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/images/revivebig.png" width="280" />
</p>

The community uses the term revive for two different concepts. The first is when a character uses an ability on another to get them out of the DOWN state, while the second is when a character is KOd and they are brought back to the match. Currently, no character can do the latter, but some can do the former. Some revive abilities are physical range, while others are long range. Reviving an ally from the DOWN state will get them back with some HP, which decreases on every revive or if the player gets up when the DOWN timer reaches zero. This HP loss per revive makes it hard for a teammate that has been revived many times to be saved from a deep point inside the Poison Mist, as at one point they'll be revived with so little HP that they'll be unable to drink even small drinks in time.

### Revivers

Characters with revive abilities. Dabi is a special case as he cannot revive others, only himself. Honorable mention to Kurogiri, who cannot revive allies directly, but can teleport them away from danger with ease and help them get up.

<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/deku_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/deku_strike.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/iida_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/froppy_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/ibara_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/allmight_assault.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/allmight_rapid.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/cementoss_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/twice_support.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/mrcompress_support.png" />
</div>

### Conditional Revivers
Characters who can only revive under certain circumstances and can't do it by default.

<div class="image-container">
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_technical.png" />
    <img class="container-image-icon" src="https://raw.githubusercontent.com/HydrosPlays/ultrarumbleguide/refs/heads/main/icons/toga_rapid.png" />
</div>

<hr style="height: 10px; background-color: white; border: none;">

<style>
    .guides-menu {
        display: flex;
        flex-direction: column;
        margin: 20px auto 20px auto; 
        justify-content: center;
        max-width: 1000px;
        gap: 15px;
        padding: 20px 20px 40px;
        margin-top: 20px;
        margin-bottom: 20px;
        background-color: #24262E;
        border-radius: 12px;
    } 
    
    .guides-menu-row {
        display: flex;
        justify-content: center;
        flex-direction: row;
        flex-wrap: wrap;
        gap: 10px;
    } 

    .guide-icon {
        flex: 0 0 auto;
        width: 175px;
        height: 175px;
        box-sizing: border-box;
    }

    .guide-icon img {
        width: 100%;
        height: 100%;
        object-fit: contain; 
    }

    @media (max-width: 768px) {
        .guide-icon {
            max-width: 75px; 
            max-height: 75px;
        }
        
        .guides-menu-row {
            gap: 5px; 
        }

        .guides-menu {
            gap: 7px; 
            padding: 10px 10px 20px;
        }
    }
</style>
