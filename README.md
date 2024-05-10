local Rayfield = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()

local Window = Rayfield:CreateWindow({
   Name = "😏 ANIME ZERO GUI V2 🤤",
   LoadingTitle = "Rayfield Interface Suite",
   LoadingSubtitle = "BY KYLE,DYLAN,LYNTON+MORE",
   ConfigurationSaving = {
      Enabled = false,
      FolderName = nil, -- Create a custom folder for your hub/game
      FileName = "ANIME ZERO GUI V2"
   },
   Discord = {
      Enabled = false,
      Invite = "noinvitelink", -- The Discord invite code, do not include discord.gg/. E.g. discord.gg/ABCD would be ABCD
      RememberJoins = true -- Set this to false to make them join the discord every time they load it up
   },
   KeySystem = true, -- Set this to true to use our key system
   KeySettings = {
      Title = "Untitled",
      Subtitle = "Key System",
      Note = "No method of obtaining the key is provided",
      FileName = "Key", -- It is recommended to use something unique as other scripts using Rayfield may overwrite your key file
      SaveKey = true, -- The user's key will be saved, but if you change the key, they will be unable to use your script
      GrabKeyFromSite = true, -- If this is true, set Key below to the RAW site you would like Rayfield to get the key from
      Key = {"https://pastebin.com/raw/rK22ZAJD"} -- List of keys that will be accepted by the system, can be RAW file links (pastebin, github etc) or simple strings ("hello","key22")
   }
})

local MainTab = Window:CreateTab("🏠", nil) -- Title, Image
local MainSection = MainTab:CreateSection("Fe scripts")

local Button = MainTab:CreateButton({
   Name = "FE fly",
   Callback = function()
   loadstring(game:HttpGet("https://scriptblox.com/raw/Universal-Script-I-Fly-gui-V3-I-6627"))()
   end,
})

local Button = MainTab:CreateButton({
   Name = "Fe bang ",
   Callback = function()
   loadstring(game:HttpGet("https://scriptblox.com/raw/bang-script(NSFW)_588"))()
   end,
})

local Button = MainTab:CreateButton({
   Name = "Fe netless",
   Callback = function()
   loadstring(game:HttpGet(('https://pastebin.com/raw/Cu7bKQWN'),true))()
   end,
})
