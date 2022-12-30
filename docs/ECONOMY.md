# Economy

- 4 Tharni = 1 Castar (useful for tax percentages)
- 1 Castar
- Gold Pice = 10 Castars
- Gold Crown = 100 Castars (♰172,800/chest)

# Plugins

## Economies

- [The new Economy](https://www.spigotmc.org/resources/the-new-economy.7805/) - Multi currency + Item Based Economy

- [Gringotts](https://www.spigotmc.org/resources/gringotts.42071/) - Item based economy

  - [gringotts-2.12.4-SNAPSHOT.jar](https://www.spigotmc.org/resources/gringotts.42071/)
  - [gringotts-towny-2.12.4-SNAPSHOT.jar](https://www.spigotmc.org/resources/gringotts-towny.105074/)
  - [Configuration](https://github.com/nikosgram/Gringotts/wiki/Configuration)

  Not compatible with `economy.closed_economy`

- GemsEconomy (QuickShop Compatible)

- TNE (QuickShop Compatible) - Multi Currency Enabled

## Shops

- [QuickShop](https://www.spigotmc.org/resources/quickshop-reremake-1-19-ready-multi-currency.62575/) - Has nice floaty
  representation of what is being sold

- [ChestShop](https://www.spigotmc.org/resources/chestshop.51856/) - 3.12.2

  - [ChestShop-towny.jar](https://www.spigotmc.org/resources/gringotts-towny.105074/) - 2.12.4-SNAPSHOT

  ```
  |              |
  |       1      |  <- How many items
  |  B 200:S 100 |  <- You can buy for $200, Sell to me for $100
  |    Diamond   |  <- Item id being sold
  |              |
  ```

# Styles of play to not break

- mining
- pvp
- adventure
- building
- village raider
- wealth accumulation

# Goals

- survival mode - Preserve the reward of acquiring materials and building things
- economy - I want the ability to trade my efforts for harder to acquire building materials
- economy opt out - Enjoy the survival minecraft experience without participating in any economy
- large builds - I should be able to build giant structures and towns if I put in the effort of mining and playing
- alive - (Encourage building near city centers)
- allow farms - afk, non-afk
- mining - should still be valuable even with AFK farms
- monster hunting - should still be a reward for monster hunting
- wealth - I want the ability to see stacks of resources in my base

# Prevent

- creative mode (Unlimited blocks kills rewarding feeling)
- stealing items (upsets players who work hard)
- griefing (frustrating when you work hard on a building only to have it destroyed)
- garbage next to your own buildings (minimum distance from a town)
- random protected garbage everywhere (wilderness?)
- Farms should not turn server into creative mode or cause economy to crash

# Potential Plugins

- Mob Bounty Reloaded - Get money for killing mobs
- Jobs -

# Econonmy Choices

- Need the ability to balance not recking the economy with the ability to get wealthy by supplying materials to the
  server.
- Purchase silk-touched ore blocks only to get around gold and iron farms...
- Allow only a certain number of items per hour to be sold
- Allow store inventory one per resident of a town. So, if there are three people in town (Joe, John, Jason), then there
  are 3 chests to fill with gold. Once Joe fills his chest with gold, he can no longer sell gold to the store but John
  and Jason can. This encourages everyone to build their own gold farm and it's not a winner take all.
- The chest/person reward decreases as each chest gets filled. this will encourage players to strategize which farms
  they want to build first.
- Tiered economy tree. You can't create shops for later tiers until you've completed the tiers that come before it.

  You have to have fully stocked shops in order to open up a new tier.

- Fix prices in the server stores to a higher price to encourage private shops. The server side store will only buy
  things if there is room, but sell them at a much higher price.

- Once a shop fills up, the shop will stop purchasing that item. This prevents farms from breaking the economy and
  rewards players for building a farm.

- Having shops enables you to build with materials that you might otherwise not acquire as quickly.

- What do you do when all your shops are full and you have no money to buy and no room to sell? What mechanism is there
  in place for someone new coming into the game to be able to use the shops? Need some sort of either a drain on the
  goods in storage or a constantly increasing money supply

- Automated Farms
- Building Anywhere
- Protecting Towns
- PVP battles

- "Reward" - An amount of money awarded to a player simply for playing.

  - Inflationary

    - Constantly increasing money supply
    - Constantly increasing prices

  - Defalationary
  - Constant Supply

    - Used as a measure for trading mining things
    - Automated farms allow users to profit

    - If we do not have rewards and set a fixed value, then

    - How do people afford to protect their homes? Forced to mine and sell goods?
    - Can we make it so the first plot is free or very cheap?

- Money Uses

  - Found a nation to enable server wars
  - Found towns to protect areas
  - Purchase town plots
  - Building Blocks
  - XP

- Problems w
- Problems with ever increasing money supply

- The number of plots a person can purchase in a town
- The ability to protect chunks in minecraft
- The ability to purchase blocks and items
- If the server has certain unlimited items for sale, then they will compete with players

- If we eliminate "reward money"

## Future

- Should cost money to move resources from one part of the world to another to allow for things to be cheaper in some
  areas

# Stores

Cost of items should be based on how long it takes to mine or acquire a thing

# Towny Pricing Strategy

We want to encourage people to participate in towns by having plots on bigger cities but then creating small hamlets or
villages for their own things.

- Make a small town affordable by one person
- Make a midsize town affordable by two people
- Make a large town affordable by 10 people

# Towny server costs

| Nation |
| ------ | ------- |
| new    | 150,000 |
| upkeep | 12,800  |

| Town                                     |        |
| ---------------------------------------- | ------ |
| new                                      | 15,000 |
| upkeep                                   | 13560  |
| claim outpost                            | 15,000 |
| claim town block                         | 2,500  |
| Town upkeep based on numberr of plots... |        |

# Player configurable costs

| Nation |       |     |
| ------ | ----- | --- |
| taxes  | Town  | 0   |
|        | Peace | 100 |

| Town          |          |        |
| ------------- | -------- | ------ |
| Price         | plot     | 1,000  |
|               | outpost  | 15,000 |
|               | shop     |        |
|               | embassy  |        |
| Taxes         | resident | 2%     |
|               | plot     | 0      |
|               | shop     | 0      |
|               | embassy  | 0      |
| Setting Plots | shop     | 50     |
|               | embassy  | 50     |
|               | wilds    | 50     |
|               | inn      | 50     |
|               | jail     | 50     |
|               | farm     | 50     |
|               | bank     | 50     |
