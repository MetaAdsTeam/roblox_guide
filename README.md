# Roblox and MetaAds integration tutorial

## Set up MetaAds Display

### Download MetaAds screen files

1. Connect to account on [MetaAds main page](https://metaads.team/main/) with Metamask.
2. Click on *Landowner*.
3. Click on *My Ad Spaces*.
4. Click on [Add Ad Space](https://metaads.team/main/publisher/my-adspaces).
5. Select Roblox metaverse.
6. Download files.
7. Click on *Next*.

![Ad Spot creation (step 1)](./images/ad_spot_section/ad_spot_creation_1.png)

8. Enter name and description.
9. Upload a preview picture, this picture will be associated with your ad spot.
10. Insert a link to the roblox image to display the default image on Ad Space, a teleport to some place triggered by click on Ad Space can be added too, if you have uploaded a default image. [How to get link to Roblox image?](#how-to-get-link-to-roblox-image)

![Ad Spot creation (step 2)](./images/ad_spot_section/ad_spot_creation_2.png)

11. Click on *Save*.

### Registration in Roblox and download of necessary environment

> Skip this section, if you have an account in Roblox, Roblox application and Roblox Studio, otherwise set up missing elements.

12. Download Roblox and Roblox Studio.
13. Register account on [Roblox](https://roblox.com).
14. Open [page for creators](https://www.roblox.com/create).
15. Click on *Start Creating* to download Roblox Studio.

![Roblox Studio downloading](./images/ad_spot_section/roblox_studio_downloading.png)

### Working in Roblox Studio

![Place creation](./images/ad_spot_section/place_creation.png)

> Skip 16th step, if you have already a place and wish set up our screen on created place.

16. Click on *New* and select template to create a new game.
17. Open your place.
18. Unzip the downloaded folder, there are the next files:

![Downloaded MetaAds archive](./images/ad_spot_section/downloaded_archive.png)

19. Open *ReplicatedStorage* folder.
20. Drag the file to Roblox Studio to *ReplicatedStorage*.
21. Open *ServerScriptService* folder.
22. Drag the file to Roblox studio to *ServerScriptService*.
23. Open *StarterGui* folder.
24. Drag the file to Roblox studio to *StarterGui*.
25. You should get the next result:

![Place's explorer](./images/ad_spot_section/place_explorer.png)

26. Copy the contents of the Environment file from downloaded files to Roblox studio: *ReplicatedStorage* -> *MetaAds* folder -> *Environment*.

![Place's environment](./images/ad_spot_section/environment.png)

### Configuration file

It consists all sizes and positions for your displays.
The next parameters are the following tables:

+ *pins*. The table of display PINs that you get after ad space creation.
+ *scales* contains available display sizes. Size a three-component variable. First and second numbers are width and height.
Third number is dummy variable and it always equals *0.01*, because display should be thin.
+ *positions* has the same dimension, but its three variables are x, y and z. The position of the display's center on all three axes.
+ *rotations*. Euler angles, the more common x, y and z notation with numbers that go from 0 to 360.
The values are set up by default if the screen is put vertically. If you wish to rotate the display forward or backward, change the first parameter. If you wish to rotate it left or right, change the second value. And if you wish to tilt left or right, use the third parameter.

27. In Roblox Studio open ReplicatedStorage.
28. Open Configuration file in MetaAds folder.
29. Go to MetaAds site, find your ad spot, open its info and get a PIN.

![Ad Spot info](./images/ad_spot_section/ad_spot_info.png)

30. Copy PIN and paste in Configuration file.

![Ad Spots configuration](./images/ad_spot_section/ad_spot_conf.png)

### Roblox game settings

31. Open *Game Settings* at *Home* tab.

![Game Settings (step 1)](./images/ad_spot_section/game_settings_1.png)

32. Click on *Save* to Roblox.

![Game Settings (step 2)](./images/ad_spot_section/game_settings_2.png)

33. Set up place's basic info: enter name and description (optional).

![Basic Info changing](./images/ad_spot_section/basic_info.png)

34. Open *Permissions* and select *Public*.

![Permissions changing](./images/ad_spot_section/permissions.png)

35. Open *Security*, ennable *Allow HTTP Requests* and *Allow Third Party Teleports*.

![Security changing](./images/ad_spot_section/security.png)

36. Click on *Save*.
37. Click on *Play* to test locally.

![MetaAds display checking](./images/ad_spot_section/display_check.png)

38. Publish to Roblox.
39. Open your game in Roblox application.

## How to get link to Roblox image?

1. Install [BTRoblox - Making Roblox Better](https://chrome.google.com/webstore/detail/btroblox-making-roblox-be/hbkpclpemjeibhioopcebchdmohaieln) extension to your browser.
2. Open page with Roblox images. They can be stored at your inventory or you can get them from common accessable [Roblox library](https://create.roblox.com/marketplace/images?source=library).

![Inventory](./images/image_section/inventory.png)
![Library](./images/image_section/library.png)

3. Select and open image.
4. Click on Explorer button.
5. Click on Decal.
6. Copy link.

![Image page](./images/image_section/image_page.png)

## How to upload your own image to Roblox?

1. Open [page for upload *Decal*](https://create.roblox.com/creations?activeTab=Decal).
2. Click on *Development items*.
3. Click on *Decals*.
4. Click on *Upload Asset*.

![Upload decal page (step 1)](./images/creative_section/upload_decal_page_1.png)

5. Click on *Upload*.
6. Select image from your PC.
7. Click on Upload button.

![Upload decal page (step 2)](./images/creative_section/upload_decal_page_2.png)

8. Wait for moderation pass.
9. Get link like [there](#how-to-get-link-to-roblox-image).

## How to upload image to MetaAds?

1. Connect on [MetaAds](https://meta-dev.eastrelay.com/main) with Metamask.
2. Click on *Advertiser*.
3. Click on *My Creatives*.
4. Click on *Add Creative*.
5. Select Roblox.
6. Paste link to Roblox image like [there](#how-to-get-link-to-roblox-image).
7. Upload preview image.

![Add Creative page](./images/creative_section/add_creative_page.png)

8. Click on Next.
9. Enter name, description and place ID (optional) to teleport by click when current creative is showing.
10. Click on Save.

![Creative parameters](./images/creative_section/creative_params.png)
