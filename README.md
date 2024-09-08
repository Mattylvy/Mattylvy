local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Window = OrionLib:MakeWindow({Name = "Miyako's Hub", HidePremium = false, SaveConfig = true, ConfigFolder = "sabe config"})

--[[
Name = <Miyako's Hub> - The name of the UI.
HidePremium = <bool> - Whether or not the user details shows Premium status or not.
SaveConfig = <bool> - Toggles the config saving in the UI.
ConfigFolder = <Trade scam  config> - The name of the folder where the configs are saved.
IntroEnabled = <bool> - Whether or not to show the intro animation.
IntroText = <welcome to Miyako's Hub> - Text to show in the intro animation.
IntroIcon = <https://cdn.discordapp.com/attachments/1120718398582702254/1282394612605911131/Screenshot_20240908-140853.png?ex=66df328d&is=66dde10d&hm=7a2bdfd535e2d84eb0d037539fbb089db67431d3e0360490ec144fe04476afe7&> - URL to the image you want to use in the intro animation.
Icon = <https://cdn.discordapp.com/attachments/1120718398582702254/1282394612605911131/Screenshot_20240908-140853.png?ex=66df328d&is=66dde10d&hm=7a2bdfd535e2d84eb0d037539fbb089db67431d3e0360490ec144fe04476afe7&> - URL to the image you want displayed on the window.
CloseCallback = <function> - Function to execute when the window is closed.
]]local Tab = Window:MakeTab({
	Name = "Tab 1",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]local Section = Tab:AddSection({
	Name = "Section"
})

--[[
Name = <string> - The name of the section.
]]OrionLib:MakeNotification({
	Name = "trade scam!",
	Content = "trade scam loaded. . .",
	Image = "rbxassetid://4483345998",
	Time = 5
})

--[[
Title = <loading script> - The title of the notification.
Content = <script finally loaded > - The content of the notification.
Image = <https://cdn.discordapp.com/attachments/1120718398582702254/1282394612605911131/Screenshot_20240908-140853.png?ex=66df328d&is=66dde10d&hm=7a2bdfd535e2d84eb0d037539fbb089db67431d3e0360490ec144fe04476afe7&> - The icon of the notification.
Time = <5> - The duration of the notfication.
]]Tab:AddButton({
	Name = "Trade Scam!",
	Callback = function()
      		print("trade scam activated")
  	end    
})

--[[
Name = <dupe pets> - The name of the button.
Callback = <Press the button to fupe your pets it doesn't work on private servers> - The function of the button.
]]OrionLib:Init()
OrionLib:Destroy()
