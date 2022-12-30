# Server Moderators and Administrators

Moderator can do what specifically?

```sh
# Create the moderator role...
lp creategroup mod
```

```sh
# Create the admin role which inherits from mod...
lp creategroup admin
lp group admin parent add mod
```

# Towny

# User Commands

```sh
# Add a user to a group
lp user jsonxr parent add mayor

# remove a user from a group
lp user jsonxr parent remove mayor
```

```sh
# default has very limited permissions...
# Anyone can login to the server to look around

# residents belong to a town and can build
lp creategroup resident
lp group resident parent add default
lp group resident permission set essentials.build true


# mayors can create towns
lp creategroup mayor
lp group mayor parent add resident
```

# Permissions descriptions

- [towny permissions](https://code.google.com/archive/a/eclipselabs.org/p/towny/wikis/PermissionNodes.wiki#:~:text=Towny%20makes%20use%20of%20Permission,By%20default%20the%20townyperms.)

- essentials.build #Works with AnitBuild to restrict people from doing anything without this
- ChestShop.shop.create.\* #Permission to create shops

# QuickShop

[online](https://www.spigotmc.org/resources/quickshop-reremake-1-19-ready-multi-currency.62575/)

## Player permissions

For lazy owners, you can use `quickshop.player` permission node to includes all permission that player need.

```yml
- quickshop.use # Required for any QuickShop Actions.
- quickshop.create.sell # Required to make a shop (Sell-Mode)
- quickshop.create.buy # Required to make a shop (Buy-Mode) or to switch from Sell to Buy-Mode.
- quickshop.create.stacks # Required to allow selling items in stacks.
- quickshop.create.changeitem # Allows a player to change a shop's item.
- quickshop.create.changeamount # Allows a player to change the item-amount per buy/sell.
- quickshop.create.changeprice # Allows a player to change the buy/sell price of their shops.
- quickshop.create.double # Allows a player to create a double chest shop.
#- quickshop.create.cmd # Required to have access to the /qs create command. This command may bypass certain protections of not-supported protection plugins!
#- quickshop.transfer # Required to transfer all owned shops to another player.
- quickshop.find # Required to use /qs find <item>
- quickshop.fetchmessage # Required to use /qs fetchmessage
- quickshop.staff # Required to use /qs staff and all its subcommands.
- quickshop.preview # Required to use the GUI Item Preview.
- quickshop.currency # Required to use the /qs currency <currency>
```

## Admin permissions

```yml
- quickshop.unlimited #Required to use /qs unlimited
- quickshop.alwayscounting #Required to use /qs alwayscounting
- quickshop.setowner #Required to use /qs setowner
- quickshop.other.destroy #Allows the player to remove/destroy shops of others.
- quickshop.other.open #Allows the player to open chests of other shops and take/put items from/into it.
- quickshop.other.price #Allows the player to change the price of someone's shop.
- quickshop.transfer.other #Required to transfer ALL shops of someone to another player.
- quickshop.refill #Allows the player to refill their shops using a command, essentially making the shop having
  unlimited items.
- quickshop.empty #Allows the player to clear the shop's inventory.
- quickshop.clean #Allows the purging/removal of any Shops that have no items in stock.
- quickshop.bypass.<ItemID> #Required to sell blacklisted items (E.g. bedrock).
- quickshop.alerts #Required to receive notifications about possible cheating, plugin warnings and updates.
- quickshop.info #Required to use /qs info
- quickshop.debug #Required to use /qs debug
- quickshop.paste #Required to use /qs paste
- quickshop.purge #Required to use /qs purge
- quickshop.create.admin #Required to bypass any protection-checks while creating a shop using /qs supercreate
- quickshop.tax #Permission to bypass the tax fee.
- quickshop.tax.bypassunlimited #Permission to bypass the tax fee but only in unlimited shop.
- quickshop.cleanghost #Permission to remove any broken shop using /qs cleanghost
- quickshop.export #Permission to use /qs export This permission is pointless since the command is console only.
- quickshop.recovery #Permission to use /qs recovery This permission is pointless since the command is console only.
- quickshop.removeworld #Permission to remove all shops in a world using /qs removeworld
- quickshop.other.changeitem #Allows the player to change the item of someone's shop.
- quickshop.other.changeamount #Allows the player to change the bulk-amount of someone's shop.
```
