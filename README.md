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

local Button = MainTab:CreateButton({
   Name = "invisible tool",
   Callback = function()
   local Players = game:GetService("Players")

local function onActivate()
    local player = Players.LocalPlayer
    local character = player.Character

    local invisible = true

    if invisible then
        for _, bodypart in pairs(character:GetChildren()) do
            if bodypart:IsA("MeshPart") or bodypart:IsA("Part") then
                bodypart.Transparency = 1
            end
        end
    end
end

local function onDeactivate()
    local player = Players.LocalPlayer
    local character = player.Character

    local invisible = false

    if not invisible then
        for _, bodypart in pairs(character:GetChildren()) do
            if bodypart.Name ~= "HumanoidRootPart" then
                if bodypart:IsA("MeshPart") or bodypart:IsA("Part") then
                    bodypart.Transparency = 0
                end
            end
        end
    end
end

local tool = Instance.new("Tool")
tool.Name = "Invisibility Tool"
tool.RequiresHandle = false
tool.Parent = Players.LocalPlayer.Backpack

tool.Activated:Connect(onActivate)
tool.Deactivated:Connect(onDeactivate)
   end,
})

local Button = MainTab:CreateButton({
   Name = "infinit yeild",
   Callback = function()
   --[[
Created by Edge
Redistributed by WeAreDevs: https://wearedevs.net/scripts

Description: A command line cheat with over 6 years of development

Instruction: Execute this script and wait for an interface to appear on your game screen.

]]

if IY_LOADED and not _G.IY_DEBUG == true then
	error("Infinite Yield is already running!",0)
	return
end

pcall(function() getgenv().IY_LOADED = true end)

if not game:IsLoaded() then
	local notLoaded = Instance.new("Message", game:GetService("CoreGui"))
	notLoaded.Text = 'Infinite Yield is waiting for the game to load'
	game.Loaded:Wait()
	notLoaded:Destroy()
end

ver = '5.6'

Players = game:GetService("Players")

Holder = Instance.new("Frame")
Title = Instance.new("TextLabel")
Dark = Instance.new("Frame")
Cmdbar = Instance.new("TextBox")
CMDsF = Instance.new("ScrollingFrame")
cmdListLayout = Instance.new("UIListLayout")
SettingsButton = Instance.new("ImageButton")
ColorsButton = Instance.new("ImageButton")
Settings = Instance.new("Frame")
Prefix = Instance.new("TextLabel")
PrefixBox = Instance.new("TextBox")
Keybinds = Instance.new("TextLabel")
StayOpen = Instance.new("TextLabel")
Button = Instance.new("Frame")
On = Instance.new("TextButton")
Positions = Instance.new("TextLabel")
EventBind = Instance.new("TextLabel")
Plugins = Instance.new("TextLabel")
Example = Instance.new("TextButton")
Notification = Instance.new("Frame")
Title_2 = Instance.new("TextLabel")
Text_2 = Instance.new("TextLabel")
CloseButton = Instance.new("TextButton")
CloseImage = Instance.new("ImageLabel")
PinButton = Instance.new("TextButton")
PinImage = Instance.new("ImageLabel")
Tooltip = Instance.new("Frame")
Title_3 = Instance.new("TextLabel")
Description = Instance.new("TextLabel")
IntroBackground = Instance.new("Frame")
Logo = Instance.new("ImageLabel")
Credits = Instance.new("TextBox")
KeybindsFrame = Instance.new("Frame")
Close = Instance.new("TextButton")
Add = Instance.new("TextButton")
Delete = Instance.new("TextButton")
Holder_2 = Instance.new("ScrollingFrame")
Example_2 = Instance.new("Frame")
Text_3 = Instance.new("TextLabel")
Delete_2 = Instance.new("TextButton")
KeybindEditor = Instance.new("Frame")
background_2 = Instance.new("Frame")
Dark_4 = Instance.new("Frame")
Directions = Instance.new("TextLabel")
BindTo = Instance.new("TextButton")
Add_2 = Instance.new("TextButton")
Cmdbar_2 = Instance.new("TextBox")
Toggles = Instance.new("ScrollingFrame")
Fly = Instance.new("TextLabel")
Select_3 = Instance.new("TextButton")
Noclip = Instance.new("TextLabel")
Select_4 = Instance.new("TextButton")
Float = Instance.new("TextLabel")
Select_5 = Instance.new("TextButton")
ClickTP = Instance.new("TextLabel")
Select_6 = Instance.new("TextButton")
ClickDelete = Instance.new("TextLabel")
Select_13 = Instance.new("TextButton") 
Xray = Instance.new("TextLabel")
Select_10 = Instance.new("TextButton")
Swim = Instance.new("TextLabel")
Select_11 = Instance.new("TextButton")
Fling = Instance.new("TextLabel")
Select_12 = Instance.new("TextButton")
Invisible = Instance.new("TextLabel")
Select_14 = Instance.new("TextButton")
Vehiclefly = Instance.new("TextLabel")
Select_15 = Instance.new("TextButton")
VehicleNoclip = Instance.new("TextLabel")
Select_16 = Instance.new("TextButton")
shadow_2 = Instance.new("Frame")
PopupText_2 = Instance.new("TextLabel")
Exit_2 = Instance.new("TextButton")
ExitImage_2 = Instance.new("ImageLabel")
PositionsFrame = Instance.new("Frame")
Close_3 = Instance.new("TextButton")
Delete_5 = Instance.new("TextButton")
Part = Instance.new("TextButton")
Holder_4 = Instance.new("ScrollingFrame")
Example_4 = Instance.new("Frame")
Text_5 = Instance.new("TextLabel")
Delete_6 = Instance.new("TextButton")
TP = Instance.new("TextButton")
AliasesFrame = Instance.new("Frame")
Close_2 = Instance.new("TextButton")
Delete_3 = Instance.new("TextButton")
Holder_3 = Instance.new("ScrollingFrame")
Example_3 = Instance.new("Frame")
Text_4 = Instance.new("TextLabel")
Delete_4 = Instance.new("TextButton")
Aliases = Instance.new("TextLabel")
PluginsFrame = Instance.new("Frame")
Close_4 = Instance.new("TextButton")
Add_3 = Instance.new("TextButton")
Holder_5 = Instance.new("ScrollingFrame")
Example_5 = Instance.new("Frame")
Text_6 = Instance.new("TextLabel")
Delete_7 = Instance.new("TextButton")
PluginEditor = Instance.new("Frame")
background_3 = Instance.new("Frame")
Dark_9 = Instance.new("Frame")
Img = Instance.new("ImageButton")
AddPlugin = Instance.new("TextButton")
FileName = Instance.new("TextBox")
About = Instance.new("TextLabel")
Directions_2 = Instance.new("TextLabel")
shadow_3 = Instance.new("Frame")
PopupText_3 = Instance.new("TextLabel")
Exit_3 = Instance.new("TextButton")
ExitImage_3 = Instance.new("ImageLabel")
AliasHint = Instance.new("TextLabel")
PluginsHint = Instance.new("TextLabel")
PositionsHint = Instance.new("TextLabel")
ToPartFrame = Instance.new("Frame")
background_5 = Instance.new("Frame")
ChoosePart = Instance.new("TextButton")
CopyPath = Instance.new("TextButton")
Directions_4 = Instance.new("TextLabel")
Path = Instance.new("TextLabel")
shadow_4 = Instance.new("Frame")
PopupText_5 = Instance.new("TextLabel")
Exit_4 = Instance.new("TextButton")
ExitImage_5 = Instance.new("ImageLabel")
logs = Instance.new("Frame")
shadow = Instance.new("Frame")
Hide = Instance.new("TextButton")
ImageLabel = Instance.new("ImageLabel")
PopupText = Instance.new("TextLabel")
Exit = Instance.new("TextButton")
ImageLabel_2 = Instance.new("ImageLabel")
background = Instance.new("Frame")
chat = Instance.new("Frame")
Clear = Instance.new("TextButton")
SaveChatlogs = Instance.new("TextButton")
Toggle = Instance.new("TextButton")
scroll_2 = Instance.new("ScrollingFrame")
join = Instance.new("Frame")
Toggle_2 = Instance.new("TextButton")
Clear_2 = Instance.new("TextButton")
scroll_3 = Instance.new("ScrollingFrame")
listlayout = Instance.new("UIListLayout",scroll_3)
selectChat = Instance.new("TextButton")
selectJoin = Instance.new("TextButton")

function randomString()
	local length = math.random(10,20)
	local array = {}
	for i = 1, length do
		array[i] = string.char(math.random(32, 126))
	end
	return table.concat(array)
end

COREGUI = game:GetService("CoreGui")
PARENT = nil
if (not is_sirhurt_closure) and (syn and syn.protect_gui) then --sirhurt is retarded
	local Main = Instance.new("ScreenGui")
	Main.Name = randomString()
	syn.protect_gui(Main)
	Main.Parent = COREGUI
	PARENT = Main
elseif get_hidden_gui or gethui then
	local hiddenUI = get_hidden_gui or gethui
	local Main = Instance.new("ScreenGui")
	Main.Name = randomString()
	Main.Parent = hiddenUI()
	PARENT = Main
elseif COREGUI:FindFirstChild('RobloxGui') then
	PARENT = COREGUI.RobloxGui
else
	local Main = Instance.new("ScreenGui")
	Main.Name = randomString()
	Main.Parent = COREGUI
	PARENT = Main
end

shade1 = {}
shade2 = {}
shade3 = {}
text1 = {}
text2 = {}
scroll = {}

Holder.Name = randomString()
Holder.Parent = PARENT
Holder.Active = true
Holder.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
Holder.BorderSizePixel = 0
Holder.Position = UDim2.new(1, -250, 1, -220)
Holder.Size = UDim2.new(0, 250, 0, 220)
Holder.ZIndex = 10
table.insert(shade2,Holder)

Title.Name = "Title"
Title.Parent = Holder
Title.Active = true
Title.BackgroundColor3 = Color3.fromRGB(36,36,37)
Title.BorderSizePixel = 0
Title.Size = UDim2.new(0, 250, 0, 20)
Title.Font = Enum.Font.SourceSans
Title.TextSize = 18
Title.Text = "Infinite Yield FE v"..ver
Title.TextColor3 = Color3.new(1, 1, 1)
Title.ZIndex = 10
table.insert(shade1,Title)
table.insert(text1,Title)

Dark.Name = "Dark"
Dark.Parent = Holder
Dark.Active = true
Dark.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
Dark.BorderSizePixel = 0
Dark.Position = UDim2.new(0, 0, 0, 45)
Dark.Size = UDim2.new(0, 250, 0, 175)
Dark.ZIndex = 10
table.insert(shade1,Dark)

Cmdbar.Name = "Cmdbar"
Cmdbar.Parent = Holder
Cmdbar.BackgroundTransparency = 1
Cmdbar.BorderSizePixel = 0
Cmdbar.Position = UDim2.new(0, 5, 0, 20)
Cmdbar.Size = UDim2.new(0, 240, 0, 25)
Cmdbar.Font = Enum.Font.SourceSans
Cmdbar.TextSize = 18
Cmdbar.TextXAlignment = Enum.TextXAlignment.Left
Cmdbar.TextColor3 = Color3.new(1, 1, 1)
Cmdbar.Text = ""
Cmdbar.ZIndex = 10
Cmdbar.PlaceholderText = "Command Bar"

CMDsF.Name = "CMDs"
CMDsF.Parent = Holder
CMDsF.BackgroundTransparency = 1
CMDsF.BorderSizePixel = 0
CMDsF.Position = UDim2.new(0, 5, 0, 45)
CMDsF.Size = UDim2.new(0, 245, 0, 175)
CMDsF.ScrollBarImageColor3 = Color3.fromRGB(78,78,79)
CMDsF.BottomImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
CMDsF.CanvasSize = UDim2.new(0, 0, 0, 0)
CMDsF.MidImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
CMDsF.ScrollBarThickness = 8
CMDsF.TopImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
CMDsF.VerticalScrollBarInset = 'Always'
CMDsF.ZIndex = 10
table.insert(scroll,CMDsF)

cmdListLayout.Parent = CMDsF

SettingsButton.Name = "SettingsButton"
SettingsButton.Parent = Holder
SettingsButton.BackgroundTransparency = 1
SettingsButton.Position = UDim2.new(0, 230, 0, 0)
SettingsButton.Size = UDim2.new(0, 20, 0, 20)
SettingsButton.Image = "rbxassetid://1204397029"
SettingsButton.ZIndex = 10

ReferenceButton = Instance.new("ImageButton")
ReferenceButton.Name = "ReferenceButton"
ReferenceButton.Parent = Holder
ReferenceButton.BackgroundTransparency = 1
ReferenceButton.Position = UDim2.new(0, 212, 0, 2)
ReferenceButton.Size = UDim2.new(0, 16, 0, 16)
ReferenceButton.Image = "rbxassetid://3523243755"
ReferenceButton.ZIndex = 10

Settings.Name = "Settings"
Settings.Parent = Holder
Settings.Active = true
Settings.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
Settings.BorderSizePixel = 0
Settings.Position = UDim2.new(0, 0, 0, 220)
Settings.Size = UDim2.new(0, 250, 0, 175)
Settings.ZIndex = 10
table.insert(shade1,Settings)

SettingsHolder = Instance.new("ScrollingFrame")
SettingsHolder.Name = "Holder"
SettingsHolder.Parent = Settings
SettingsHolder.BackgroundTransparency = 1
SettingsHolder.BorderSizePixel = 0
SettingsHolder.Size = UDim2.new(1,0,1,0)
SettingsHolder.ScrollBarImageColor3 = Color3.fromRGB(78,78,79)
SettingsHolder.BottomImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
SettingsHolder.CanvasSize = UDim2.new(0, 0, 0, 235)
SettingsHolder.MidImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
SettingsHolder.ScrollBarThickness = 8
SettingsHolder.TopImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
SettingsHolder.VerticalScrollBarInset = 'Always'
SettingsHolder.ZIndex = 10
table.insert(scroll,SettingsHolder)

Prefix.Name = "Prefix"
Prefix.Parent = SettingsHolder
Prefix.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
Prefix.BorderSizePixel = 0
Prefix.BackgroundTransparency = 1
Prefix.Position = UDim2.new(0, 5, 0, 5)
Prefix.Size = UDim2.new(1, -10, 0, 20)
Prefix.Font = Enum.Font.SourceSans
Prefix.TextSize = 14
Prefix.Text = "Prefix"
Prefix.TextColor3 = Color3.new(1, 1, 1)
Prefix.TextXAlignment = Enum.TextXAlignment.Left
Prefix.ZIndex = 10
table.insert(shade2,Prefix)
table.insert(text1,Prefix)

PrefixBox.Name = "PrefixBox"
PrefixBox.Parent = Prefix
PrefixBox.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
PrefixBox.BorderSizePixel = 0
PrefixBox.Position = UDim2.new(1, -20, 0, 0)
PrefixBox.Size = UDim2.new(0, 20, 0, 20)
PrefixBox.Font = Enum.Font.SourceSansBold
PrefixBox.TextSize = 14
PrefixBox.Text = ''
PrefixBox.TextColor3 = Color3.new(0, 0, 0)
PrefixBox.ZIndex = 10
table.insert(shade3,PrefixBox)
table.insert(text2,PrefixBox)

function makeSettingsButton(name,iconID,off)
	local button = Instance.new("TextButton")
	button.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	button.BorderSizePixel = 0
	button.Position = UDim2.new(0,0,0,0)
	button.Size = UDim2.new(1,0,0,25)
	button.Text = ""
	button.ZIndex = 10
	local icon = Instance.new("ImageLabel")
	icon.Name = "Icon"
	icon.Parent = button
	icon.Position = UDim2.new(0,5,0,5)
	icon.Size = UDim2.new(0,16,0,16)
	icon.BackgroundTransparency = 1
	icon.Image = iconID
	icon.ZIndex = 10
	if off then
		icon.ScaleType = Enum.ScaleType.Crop
		icon.ImageRectSize = Vector2.new(16,16)
		icon.ImageRectOffset = Vector2.new(off,0)
	end
	local label = Instance.new("TextLabel")
	label.Name = "ButtonLabel"
	label.Parent = button
	label.BackgroundTransparency = 1
	label.Text = name
	label.Position = UDim2.new(0,28,0,0)
	label.Size = UDim2.new(1,-28,1,0)
	label.Font = Enum.Font.SourceSans
	label.TextColor3 = Color3.new(1, 1, 1)
	label.TextSize = 14
	label.ZIndex = 10
	label.TextXAlignment = Enum.TextXAlignment.Left
	table.insert(shade2,button)
	table.insert(text1,label)
	return button
end

ColorsButton = makeSettingsButton("Edit Theme","rbxassetid://4911962991")
ColorsButton.Position = UDim2.new(0,5,0,55)
ColorsButton.Size = UDim2.new(1,-10,0,25)
ColorsButton.Name = "Colors"
ColorsButton.Parent = SettingsHolder

Keybinds = makeSettingsButton("Edit Keybinds","rbxassetid://129697930")
Keybinds.Position = UDim2.new(0, 5, 0, 85)
Keybinds.Size = UDim2.new(1, -10, 0, 25)
Keybinds.Name = "Keybinds"
Keybinds.Parent = SettingsHolder

Aliases = makeSettingsButton("Edit Aliases","rbxassetid://5147488658")
Aliases.Position = UDim2.new(0, 5, 0, 115)
Aliases.Size = UDim2.new(1, -10, 0, 25)
Aliases.Name = "Aliases"
Aliases.Parent = SettingsHolder

StayOpen.Name = "StayOpen"
StayOpen.Parent = SettingsHolder
StayOpen.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
StayOpen.BorderSizePixel = 0
StayOpen.BackgroundTransparency = 1
StayOpen.Position = UDim2.new(0, 5, 0, 30)
StayOpen.Size = UDim2.new(1, -10, 0, 20)
StayOpen.Font = Enum.Font.SourceSans
StayOpen.TextSize = 14
StayOpen.Text = "Keep Menu Open"
StayOpen.TextColor3 = Color3.new(1, 1, 1)
StayOpen.TextXAlignment = Enum.TextXAlignment.Left
StayOpen.ZIndex = 10
table.insert(shade2,StayOpen)
table.insert(text1,StayOpen)

Button.Name = "Button"
Button.Parent = StayOpen
Button.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
Button.BorderSizePixel = 0
Button.Position = UDim2.new(1, -20, 0, 0)
Button.Size = UDim2.new(0, 20, 0, 20)
Button.ZIndex = 10
table.insert(shade3,Button)

On.Name = "On"
On.Parent = Button
On.BackgroundColor3 = Color3.fromRGB(150, 150, 151)
On.BackgroundTransparency = 1
On.BorderSizePixel = 0
On.Position = UDim2.new(0, 2, 0, 2)
On.Size = UDim2.new(0, 16, 0, 16)
On.Font = Enum.Font.SourceSans
On.FontSize = Enum.FontSize.Size14
On.Text = ""
On.TextColor3 = Color3.new(0, 0, 0)
On.ZIndex = 10

Positions = makeSettingsButton("Edit/Goto Waypoints","rbxassetid://5147488592")
Positions.Position = UDim2.new(0, 5, 0, 145)
Positions.Size = UDim2.new(1, -10, 0, 25)
Positions.Name = "Waypoints"
Positions.Parent = SettingsHolder

EventBind = makeSettingsButton("Edit Event Binds","rbxassetid://5147695474",759)
EventBind.Position = UDim2.new(0, 5, 0, 205)
EventBind.Size = UDim2.new(1, -10, 0, 25)
EventBind.Name = "EventBinds"
EventBind.Parent = SettingsHolder

Plugins = makeSettingsButton("Manage Plugins","rbxassetid://5147695474",743)
Plugins.Position = UDim2.new(0, 5, 0, 175)
Plugins.Size = UDim2.new(1, -10, 0, 25)
Plugins.Name = "Plugins"
Plugins.Parent = SettingsHolder

Example.Name = "Example"
Example.Parent = Holder
Example.BackgroundTransparency = 1
Example.BorderSizePixel = 0
Example.Size = UDim2.new(0, 190, 0, 20)
Example.Visible = false
Example.Font = Enum.Font.SourceSans
Example.TextSize = 18
Example.Text = "Example"
Example.TextColor3 = Color3.new(1, 1, 1)
Example.TextXAlignment = Enum.TextXAlignment.Left
Example.ZIndex = 10
table.insert(text1,Example)

Notification.Name = randomString()
Notification.Parent = PARENT
Notification.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
Notification.BorderSizePixel = 0
Notification.Position = UDim2.new(1, -500, 1, 20)
Notification.Size = UDim2.new(0, 250, 0, 100)
Notification.ZIndex = 10
table.insert(shade1,Notification)

Title_2.Name = "Title"
Title_2.Parent = Notification
Title_2.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
Title_2.BorderSizePixel = 0
Title_2.Size = UDim2.new(0, 250, 0, 20)
Title_2.Font = Enum.Font.SourceSans
Title_2.TextSize = 14
Title_2.Text = "Notification Title"
Title_2.TextColor3 = Color3.new(1, 1, 1)
Title_2.ZIndex = 10
table.insert(shade2,Title_2)
table.insert(text1,Title_2)

Text_2.Name = "Text"
Text_2.Parent = Notification
Text_2.BackgroundTransparency = 1
Text_2.BorderSizePixel = 0
Text_2.Position = UDim2.new(0, 5, 0, 25)
Text_2.Size = UDim2.new(0, 240, 0, 75)
Text_2.Font = Enum.Font.SourceSans
Text_2.TextSize = 16
Text_2.Text = "Notification Text"
Text_2.TextColor3 = Color3.new(1, 1, 1)
Text_2.TextWrapped = true
Text_2.ZIndex = 10
table.insert(text1,Text_2)

CloseButton.Name = "CloseButton"
CloseButton.Parent = Notification
CloseButton.BackgroundTransparency = 1
CloseButton.Position = UDim2.new(1, -20, 0, 0)
CloseButton.Size = UDim2.new(0, 20, 0, 20)
CloseButton.Text = ""
CloseButton.ZIndex = 10

CloseImage.Parent = CloseButton
CloseImage.BackgroundColor3 = Color3.new(1, 1, 1)
CloseImage.BackgroundTransparency = 1
CloseImage.Position = UDim2.new(0, 5, 0, 5)
CloseImage.Size = UDim2.new(0, 10, 0, 10)
CloseImage.Image = "rbxassetid://5054663650"
CloseImage.ZIndex = 10

PinButton.Name = "PinButton"
PinButton.Parent = Notification
PinButton.BackgroundTransparency = 1
PinButton.Size = UDim2.new(0, 20, 0, 20)
PinButton.ZIndex = 10
PinButton.Text = ""

PinImage.Parent = PinButton
PinImage.BackgroundColor3 = Color3.new(1, 1, 1)
PinImage.BackgroundTransparency = 1
PinImage.Position = UDim2.new(0, 3, 0, 3)
PinImage.Size = UDim2.new(0, 14, 0, 14)
PinImage.ZIndex = 10
PinImage.Image = "rbxassetid://6234691350"

Tooltip.Name = randomString()
Tooltip.Parent = PARENT
Tooltip.Active = true
Tooltip.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
Tooltip.BackgroundTransparency = 0.1
Tooltip.BorderSizePixel = 0
Tooltip.Size = UDim2.new(0, 200, 0, 96)
Tooltip.Visible = false
Tooltip.ZIndex = 10
table.insert(shade1,Tooltip)

Title_3.Name = "Title"
Title_3.Parent = Tooltip
Title_3.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
Title_3.BackgroundTransparency = 0.1
Title_3.BorderSizePixel = 0
Title_3.Size = UDim2.new(0, 200, 0, 20)
Title_3.Font = Enum.Font.SourceSans
Title_3.TextSize = 14
Title_3.Text = ""
Title_3.TextColor3 = Color3.new(1, 1, 1)
Title_3.TextTransparency = 0.1
Title_3.ZIndex = 10
table.insert(shade2,Title_3)
table.insert(text1,Title_3)

Description.Name = "Description"
Description.Parent = Tooltip
Description.BackgroundTransparency = 1
Description.BorderSizePixel = 0
Description.Size = UDim2.new(0,180,0,72)
Description.Position = UDim2.new(0,10,0,18)
Description.Font = Enum.Font.SourceSans
Description.TextSize = 16
Description.Text = ""
Description.TextColor3 = Color3.new(1, 1, 1)
Description.TextTransparency = 0.1
Description.TextWrapped = true
Description.ZIndex = 10
table.insert(text1,Description)

IntroBackground.Name = "IntroBackground"
IntroBackground.Parent = Holder
IntroBackground.Active = true
IntroBackground.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
IntroBackground.BorderSizePixel = 0
IntroBackground.Position = UDim2.new(0, 0, 0, 45)
IntroBackground.Size = UDim2.new(0, 250, 0, 175)
IntroBackground.ZIndex = 10

Logo.Name = "Logo"
Logo.Parent = Holder
Logo.BackgroundTransparency = 1
Logo.BorderSizePixel = 0
Logo.Position = UDim2.new(0, 125, 0, 127)
Logo.Size = UDim2.new(0, 10, 0, 10)
Logo.Image = "rbxassetid://1352543873"
Logo.ImageTransparency = 0
Logo.ZIndex = 10

Credits.Name = "Credits"
Credits.Parent = Holder
Credits.BackgroundTransparency = 1
Credits.BorderSizePixel = 0
Credits.Position = UDim2.new(0, 0, 0.9, 30)
Credits.Size = UDim2.new(0, 250, 0, 20)
Credits.Font = Enum.Font.SourceSansLight
Credits.FontSize = Enum.FontSize.Size18
Credits.Text = "Edge // Zwolf // Moon // Toon"
Credits.TextColor3 = Color3.new(1, 1, 1)
Credits.ZIndex = 10

KeybindsFrame.Name = "KeybindsFrame"
KeybindsFrame.Parent = Settings
KeybindsFrame.Active = true
KeybindsFrame.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
KeybindsFrame.BorderSizePixel = 0
KeybindsFrame.Position = UDim2.new(0, 0, 0, 175)
KeybindsFrame.Size = UDim2.new(0, 250, 0, 175)
KeybindsFrame.ZIndex = 10
table.insert(shade1,KeybindsFrame)

Close.Name = "Close"
Close.Parent = KeybindsFrame
Cl--[[
Created by Edge
Redistributed by WeAreDevs: https://wearedevs.net/scripts

Description: A command line cheat with over 6 years of development

Instruction: Execute this script and wait for an interface to appear on your game screen.

]]

if IY_LOADED and not _G.IY_DEBUG == true then
	error("Infinite Yield is already running!",0)
	return
end

pcall(function() getgenv().IY_LOADED = true end)

if not game:IsLoaded() then
	local notLoaded = Instance.new("Message", game:GetService("CoreGui"))
	notLoaded.Text = 'Infinite Yield is waiting for the game to load'
	game.Loaded:Wait()
	notLoaded:Destroy()
end

ver = '5.6'

Players = game:GetService("Players")

Holder = Instance.new("Frame")
Title = Instance.new("TextLabel")
Dark = Instance.new("Frame")
Cmdbar = Instance.new("TextBox")
CMDsF = Instance.new("ScrollingFrame")
cmdListLayout = Instance.new("UIListLayout")
SettingsButton = Instance.new("ImageButton")
ColorsButton = Instance.new("ImageButton")
Settings = Instance.new("Frame")
Prefix = Instance.new("TextLabel")
PrefixBox = Instance.new("TextBox")
Keybinds = Instance.new("TextLabel")
StayOpen = Instance.new("TextLabel")
Button = Instance.new("Frame")
On = Instance.new("TextButton")
Positions = Instance.new("TextLabel")
EventBind = Instance.new("TextLabel")
Plugins = Instance.new("TextLabel")
Example = Instance.new("TextButton")
Notification = Instance.new("Frame")
Title_2 = Instance.new("TextLabel")
Text_2 = Instance.new("TextLabel")
CloseButton = Instance.new("TextButton")
CloseImage = Instance.new("ImageLabel")
PinButton = Instance.new("TextButton")
PinImage = Instance.new("ImageLabel")
Tooltip = Instance.new("Frame")
Title_3 = Instance.new("TextLabel")
Description = Instance.new("TextLabel")
IntroBackground = Instance.new("Frame")
Logo = Instance.new("ImageLabel")
Credits = Instance.new("TextBox")
KeybindsFrame = Instance.new("Frame")
Close = Instance.new("TextButton")
Add = Instance.new("TextButton")
Delete = Instance.new("TextButton")
Holder_2 = Instance.new("ScrollingFrame")
Example_2 = Instance.new("Frame")
Text_3 = Instance.new("TextLabel")
Delete_2 = Instance.new("TextButton")
KeybindEditor = Instance.new("Frame")
background_2 = Instance.new("Frame")
Dark_4 = Instance.new("Frame")
Directions = Instance.new("TextLabel")
BindTo = Instance.new("TextButton")
Add_2 = Instance.new("TextButton")
Cmdbar_2 = Instance.new("TextBox")
Toggles = Instance.new("ScrollingFrame")
Fly = Instance.new("TextLabel")
Select_3 = Instance.new("TextButton")
Noclip = Instance.new("TextLabel")
Select_4 = Instance.new("TextButton")
Float = Instance.new("TextLabel")
Select_5 = Instance.new("TextButton")
ClickTP = Instance.new("TextLabel")
Select_6 = Instance.new("TextButton")
ClickDelete = Instance.new("TextLabel")
Select_13 = Instance.new("TextButton") 
Xray = Instance.new("TextLabel")
Select_10 = Instance.new("TextButton")
Swim = Instance.new("TextLabel")
Select_11 = Instance.new("TextButton")
Fling = Instance.new("TextLabel")
Select_12 = Instance.new("TextButton")
Invisible = Instance.new("TextLabel")
Select_14 = Instance.new("TextButton")
Vehiclefly = Instance.new("TextLabel")
Select_15 = Instance.new("TextButton")
VehicleNoclip = Instance.new("TextLabel")
Select_16 = Instance.new("TextButton")
shadow_2 = Instance.new("Frame")
PopupText_2 = Instance.new("TextLabel")
Exit_2 = Instance.new("TextButton")
ExitImage_2 = Instance.new("ImageLabel")
PositionsFrame = Instance.new("Frame")
Close_3 = Instance.new("TextButton")
Delete_5 = Instance.new("TextButton")
Part = Instance.new("TextButton")
Holder_4 = Instance.new("ScrollingFrame")
Example_4 = Instance.new("Frame")
Text_5 = Instance.new("TextLabel")
Delete_6 = Instance.new("TextButton")
TP = Instance.new("TextButton")
AliasesFrame = Instance.new("Frame")
Close_2 = Instance.new("TextButton")
Delete_3 = Instance.new("TextButton")
Holder_3 = Instance.new("ScrollingFrame")
Example_3 = Instance.new("Frame")
Text_4 = Instance.new("TextLabel")
Delete_4 = Instance.new("TextButton")
Aliases = Instance.new("TextLabel")
PluginsFrame = Instance.new("Frame")
Close_4 = Instance.new("TextButton")
Add_3 = Instance.new("TextButton")
Holder_5 = Instance.new("ScrollingFrame")
Example_5 = Instance.new("Frame")
Text_6 = Instance.new("TextLabel")
Delete_7 = Instance.new("TextButton")
PluginEditor = Instance.new("Frame")
background_3 = Instance.new("Frame")
Dark_9 = Instance.new("Frame")
Img = Instance.new("ImageButton")
AddPlugin = Instance.new("TextButton")
FileName = Instance.new("TextBox")
About = Instance.new("TextLabel")
Directions_2 = Instance.new("TextLabel")
shadow_3 = Instance.new("Frame")
PopupText_3 = Instance.new("TextLabel")
Exit_3 = Instance.new("TextButton")
ExitImage_3 = Instance.new("ImageLabel")
AliasHint = Instance.new("TextLabel")
PluginsHint = Instance.new("TextLabel")
PositionsHint = Instance.new("TextLabel")
ToPartFrame = Instance.new("Frame")
background_5 = Instance.new("Frame")
ChoosePart = Instance.new("TextButton")
CopyPath = Instance.new("TextButton")
Directions_4 = Instance.new("TextLabel")
Path = Instance.new("TextLabel")
shadow_4 = Instance.new("Frame")
PopupText_5 = Instance.new("TextLabel")
Exit_4 = Instance.new("TextButton")
ExitImage_5 = Instance.new("ImageLabel")
logs = Instance.new("Frame")
shadow = Instance.new("Frame")
Hide = Instance.new("TextButton")
ImageLabel = Instance.new("ImageLabel")
PopupText = Instance.new("TextLabel")
Exit = Instance.new("TextButton")
ImageLabel_2 = Instance.new("ImageLabel")
background = Instance.new("Frame")
chat = Instance.new("Frame")
Clear = Instance.new("TextButton")
SaveChatlogs = Instance.new("TextButton")
Toggle = Instance.new("TextButton")
scroll_2 = Instance.new("ScrollingFrame")
join = Instance.new("Frame")
Toggle_2 = Instance.new("TextButton")
Clear_2 = Instance.new("TextButton")
scroll_3 = Instance.new("ScrollingFrame")
listlayout = Instance.new("UIListLayout",scroll_3)
selectChat = Instance.new("TextButton")
selectJoin = Instance.new("TextButton")

function randomString()
	local length = math.random(10,20)
	local array = {}
	for i = 1, length do
		array[i] = string.char(math.random(32, 126))
	end
	return table.concat(array)
end

COREGUI = game:GetService("CoreGui")
PARENT = nil
if (not is_sirhurt_closure) and (syn and syn.protect_gui) then --sirhurt is retarded
	local Main = Instance.new("ScreenGui")
	Main.Name = randomString()
	syn.protect_gui(Main)
	Main.Parent = COREGUI
	PARENT = Main
elseif get_hidden_gui or gethui then
	local hiddenUI = get_hidden_gui or gethui
	local Main = Instance.new("ScreenGui")
	Main.Name = randomString()
	Main.Parent = hiddenUI()
	PARENT = Main
elseif COREGUI:FindFirstChild('RobloxGui') then
	PARENT = COREGUI.RobloxGui
else
	local Main = Instance.new("ScreenGui")
	Main.Name = randomString()
	Main.Parent = COREGUI
	PARENT = Main
end

shade1 = {}
shade2 = {}
shade3 = {}
text1 = {}
text2 = {}
scroll = {}

Holder.Name = randomString()
Holder.Parent = PARENT
Holder.Active = true
Holder.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
Holder.BorderSizePixel = 0
Holder.Position = UDim2.new(1, -250, 1, -220)
Holder.Size = UDim2.new(0, 250, 0, 220)
Holder.ZIndex = 10
table.insert(shade2,Holder)

Title.Name = "Title"
Title.Parent = Holder
Title.Active = true
Title.BackgroundColor3 = Color3.fromRGB(36,36,37)
Title.BorderSizePixel = 0
Title.Size = UDim2.new(0, 250, 0, 20)
Title.Font = Enum.Font.SourceSans
Title.TextSize = 18
Title.Text = "Infinite Yield FE v"..ver
Title.TextColor3 = Color3.new(1, 1, 1)
Title.ZIndex = 10
table.insert(shade1,Title)
table.insert(text1,Title)

Dark.Name = "Dark"
Dark.Parent = Holder
Dark.Active = true
Dark.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
Dark.BorderSizePixel = 0
Dark.Position = UDim2.new(0, 0, 0, 45)
Dark.Size = UDim2.new(0, 250, 0, 175)
Dark.ZIndex = 10
table.insert(shade1,Dark)

Cmdbar.Name = "Cmdbar"
Cmdbar.Parent = Holder
Cmdbar.BackgroundTransparency = 1
Cmdbar.BorderSizePixel = 0
Cmdbar.Position = UDim2.new(0, 5, 0, 20)
Cmdbar.Size = UDim2.new(0, 240, 0, 25)
Cmdbar.Font = Enum.Font.SourceSans
Cmdbar.TextSize = 18
Cmdbar.TextXAlignment = Enum.TextXAlignment.Left
Cmdbar.TextColor3 = Color3.new(1, 1, 1)
Cmdbar.Text = ""
Cmdbar.ZIndex = 10
Cmdbar.PlaceholderText = "Command Bar"

CMDsF.Name = "CMDs"
CMDsF.Parent = Holder
CMDsF.BackgroundTransparency = 1
CMDsF.BorderSizePixel = 0
CMDsF.Position = UDim2.new(0, 5, 0, 45)
CMDsF.Size = UDim2.new(0, 245, 0, 175)
CMDsF.ScrollBarImageColor3 = Color3.fromRGB(78,78,79)
CMDsF.BottomImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
CMDsF.CanvasSize = UDim2.new(0, 0, 0, 0)
CMDsF.MidImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
CMDsF.ScrollBarThickness = 8
CMDsF.TopImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
CMDsF.VerticalScrollBarInset = 'Always'
CMDsF.ZIndex = 10
table.insert(scroll,CMDsF)

cmdListLayout.Parent = CMDsF

SettingsButton.Name = "SettingsButton"
SettingsButton.Parent = Holder
SettingsButton.BackgroundTransparency = 1
SettingsButton.Position = UDim2.new(0, 230, 0, 0)
SettingsButton.Size = UDim2.new(0, 20, 0, 20)
SettingsButton.Image = "rbxassetid://1204397029"
SettingsButton.ZIndex = 10

ReferenceButton = Instance.new("ImageButton")
ReferenceButton.Name = "ReferenceButton"
ReferenceButton.Parent = Holder
ReferenceButton.BackgroundTransparency = 1
ReferenceButton.Position = UDim2.new(0, 212, 0, 2)
ReferenceButton.Size = UDim2.new(0, 16, 0, 16)
ReferenceButton.Image = "rbxassetid://3523243755"
ReferenceButton.ZIndex = 10

Settings.Name = "Settings"
Settings.Parent = Holder
Settings.Active = true
Settings.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
Settings.BorderSizePixel = 0
Settings.Position = UDim2.new(0, 0, 0, 220)
Settings.Size = UDim2.new(0, 250, 0, 175)
Settings.ZIndex = 10
table.insert(shade1,Settings)

SettingsHolder = Instance.new("ScrollingFrame")
SettingsHolder.Name = "Holder"
SettingsHolder.Parent = Settings
SettingsHolder.BackgroundTransparency = 1
SettingsHolder.BorderSizePixel = 0
SettingsHolder.Size = UDim2.new(1,0,1,0)
SettingsHolder.ScrollBarImageColor3 = Color3.fromRGB(78,78,79)
SettingsHolder.BottomImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
SettingsHolder.CanvasSize = UDim2.new(0, 0, 0, 235)
SettingsHolder.MidImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
SettingsHolder.ScrollBarThickness = 8
SettingsHolder.TopImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
SettingsHolder.VerticalScrollBarInset = 'Always'
SettingsHolder.ZIndex = 10
table.insert(scroll,SettingsHolder)

Prefix.Name = "Prefix"
Prefix.Parent = SettingsHolder
Prefix.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
Prefix.BorderSizePixel = 0
Prefix.BackgroundTransparency = 1
Prefix.Position = UDim2.new(0, 5, 0, 5)
Prefix.Size = UDim2.new(1, -10, 0, 20)
Prefix.Font = Enum.Font.SourceSans
Prefix.TextSize = 14
Prefix.Text = "Prefix"
Prefix.TextColor3 = Color3.new(1, 1, 1)
Prefix.TextXAlignment = Enum.TextXAlignment.Left
Prefix.ZIndex = 10
table.insert(shade2,Prefix)
table.insert(text1,Prefix)

PrefixBox.Name = "PrefixBox"
PrefixBox.Parent = Prefix
PrefixBox.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
PrefixBox.BorderSizePixel = 0
PrefixBox.Position = UDim2.new(1, -20, 0, 0)
PrefixBox.Size = UDim2.new(0, 20, 0, 20)
PrefixBox.Font = Enum.Font.SourceSansBold
PrefixBox.TextSize = 14
PrefixBox.Text = ''
PrefixBox.TextColor3 = Color3.new(0, 0, 0)
PrefixBox.ZIndex = 10
table.insert(shade3,PrefixBox)
table.insert(text2,PrefixBox)

function makeSettingsButton(name,iconID,off)
	local button = Instance.new("TextButton")
	button.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
	button.BorderSizePixel = 0
	button.Position = UDim2.new(0,0,0,0)
	button.Size = UDim2.new(1,0,0,25)
	button.Text = ""
	button.ZIndex = 10
	local icon = Instance.new("ImageLabel")
	icon.Name = "Icon"
	icon.Parent = button
	icon.Position = UDim2.new(0,5,0,5)
	icon.Size = UDim2.new(0,16,0,16)
	icon.BackgroundTransparency = 1
	icon.Image = iconID
	icon.ZIndex = 10
	if off then
		icon.ScaleType = Enum.ScaleType.Crop
		icon.ImageRectSize = Vector2.new(16,16)
		icon.ImageRectOffset = Vector2.new(off,0)
	end
	local label = Instance.new("TextLabel")
	label.Name = "ButtonLabel"
	label.Parent = button
	label.BackgroundTransparency = 1
	label.Text = name
	label.Position = UDim2.new(0,28,0,0)
	label.Size = UDim2.new(1,-28,1,0)
	label.Font = Enum.Font.SourceSans
	label.TextColor3 = Color3.new(1, 1, 1)
	label.TextSize = 14
	label.ZIndex = 10
	label.TextXAlignment = Enum.TextXAlignment.Left
	table.insert(shade2,button)
	table.insert(text1,label)
	return button
end

ColorsButton = makeSettingsButton("Edit Theme","rbxassetid://4911962991")
ColorsButton.Position = UDim2.new(0,5,0,55)
ColorsButton.Size = UDim2.new(1,-10,0,25)
ColorsButton.Name = "Colors"
ColorsButton.Parent = SettingsHolder

Keybinds = makeSettingsButton("Edit Keybinds","rbxassetid://129697930")
Keybinds.Position = UDim2.new(0, 5, 0, 85)
Keybinds.Size = UDim2.new(1, -10, 0, 25)
Keybinds.Name = "Keybinds"
Keybinds.Parent = SettingsHolder

Aliases = makeSettingsButton("Edit Aliases","rbxassetid://5147488658")
Aliases.Position = UDim2.new(0, 5, 0, 115)
Aliases.Size = UDim2.new(1, -10, 0, 25)
Aliases.Name = "Aliases"
Aliases.Parent = SettingsHolder

StayOpen.Name = "StayOpen"
StayOpen.Parent = SettingsHolder
StayOpen.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
StayOpen.BorderSizePixel = 0
StayOpen.BackgroundTransparency = 1
StayOpen.Position = UDim2.new(0, 5, 0, 30)
StayOpen.Size = UDim2.new(1, -10, 0, 20)
StayOpen.Font = Enum.Font.SourceSans
StayOpen.TextSize = 14
StayOpen.Text = "Keep Menu Open"
StayOpen.TextColor3 = Color3.new(1, 1, 1)
StayOpen.TextXAlignment = Enum.TextXAlignment.Left
StayOpen.ZIndex = 10
table.insert(shade2,StayOpen)
table.insert(text1,StayOpen)

Button.Name = "Button"
Button.Parent = StayOpen
Button.BackgroundColor3 = Color3.fromRGB(78, 78, 79)
Button.BorderSizePixel = 0
Button.Position = UDim2.new(1, -20, 0, 0)
Button.Size = UDim2.new(0, 20, 0, 20)
Button.ZIndex = 10
table.insert(shade3,Button)

On.Name = "On"
On.Parent = Button
On.BackgroundColor3 = Color3.fromRGB(150, 150, 151)
On.BackgroundTransparency = 1
On.BorderSizePixel = 0
On.Position = UDim2.new(0, 2, 0, 2)
On.Size = UDim2.new(0, 16, 0, 16)
On.Font = Enum.Font.SourceSans
On.FontSize = Enum.FontSize.Size14
On.Text = ""
On.TextColor3 = Color3.new(0, 0, 0)
On.ZIndex = 10

Positions = makeSettingsButton("Edit/Goto Waypoints","rbxassetid://5147488592")
Positions.Position = UDim2.new(0, 5, 0, 145)
Positions.Size = UDim2.new(1, -10, 0, 25)
Positions.Name = "Waypoints"
Positions.Parent = SettingsHolder

EventBind = makeSettingsButton("Edit Event Binds","rbxassetid://5147695474",759)
EventBind.Position = UDim2.new(0, 5, 0, 205)
EventBind.Size = UDim2.new(1, -10, 0, 25)
EventBind.Name = "EventBinds"
EventBind.Parent = SettingsHolder

Plugins = makeSettingsButton("Manage Plugins","rbxassetid://5147695474",743)
Plugins.Position = UDim2.new(0, 5, 0, 175)
Plugins.Size = UDim2.new(1, -10, 0, 25)
Plugins.Name = "Plugins"
Plugins.Parent = SettingsHolder

Example.Name = "Example"
Example.Parent = Holder
Example.BackgroundTransparency = 1
Example.BorderSizePixel = 0
Example.Size = UDim2.new(0, 190, 0, 20)
Example.Visible = false
Example.Font = Enum.Font.SourceSans
Example.TextSize = 18
Example.Text = "Example"
Example.TextColor3 = Color3.new(1, 1, 1)
Example.TextXAlignment = Enum.TextXAlignment.Left
Example.ZIndex = 10
table.insert(text1,Example)

Notification.Name = randomString()
Notification.Parent = PARENT
Notification.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
Notification.BorderSizePixel = 0
Notification.Position = UDim2.new(1, -500, 1, 20)
Notification.Size = UDim2.new(0, 250, 0, 100)
Notification.ZIndex = 10
table.insert(shade1,Notification)

Title_2.Name = "Title"
Title_2.Parent = Notification
Title_2.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
Title_2.BorderSizePixel = 0
Title_2.Size = UDim2.new(0, 250, 0, 20)
Title_2.Font = Enum.Font.SourceSans
Title_2.TextSize = 14
Title_2.Text = "Notification Title"
Title_2.TextColor3 = Color3.new(1, 1, 1)
Title_2.ZIndex = 10
table.insert(shade2,Title_2)
table.insert(text1,Title_2)

Text_2.Name = "Text"
Text_2.Parent = Notification
Text_2.BackgroundTransparency = 1
Text_2.BorderSizePixel = 0
Text_2.Position = UDim2.new(0, 5, 0, 25)
Text_2.Size = UDim2.new(0, 240, 0, 75)
Text_2.Font = Enum.Font.SourceSans
Text_2.TextSize = 16
Text_2.Text = "Notification Text"
Text_2.TextColor3 = Color3.new(1, 1, 1)
Text_2.TextWrapped = true
Text_2.ZIndex = 10
table.insert(text1,Text_2)

CloseButton.Name = "CloseButton"
CloseButton.Parent = Notification
CloseButton.BackgroundTransparency = 1
CloseButton.Position = UDim2.new(1, -20, 0, 0)
CloseButton.Size = UDim2.new(0, 20, 0, 20)
CloseButton.Text = ""
CloseButton.ZIndex = 10

CloseImage.Parent = CloseButton
CloseImage.BackgroundColor3 = Color3.new(1, 1, 1)
CloseImage.BackgroundTransparency = 1
CloseImage.Position = UDim2.new(0, 5, 0, 5)
CloseImage.Size = UDim2.new(0, 10, 0, 10)
CloseImage.Image = "rbxassetid://5054663650"
CloseImage.ZIndex = 10

PinButton.Name = "PinButton"
PinButton.Parent = Notification
PinButton.BackgroundTransparency = 1
PinButton.Size = UDim2.new(0, 20, 0, 20)
PinButton.ZIndex = 10
PinButton.Text = ""

PinImage.Parent = PinButton
PinImage.BackgroundColor3 = Color3.new(1, 1, 1)
PinImage.BackgroundTransparency = 1
PinImage.Position = UDim2.new(0, 3, 0, 3)
PinImage.Size = UDim2.new(0, 14, 0, 14)
PinImage.ZIndex = 10
PinImage.Image = "rbxassetid://6234691350"

Tooltip.Name = randomString()
Tooltip.Parent = PARENT
Tooltip.Active = true
Tooltip.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
Tooltip.BackgroundTransparency = 0.1
Tooltip.BorderSizePixel = 0
Tooltip.Size = UDim2.new(0, 200, 0, 96)
Tooltip.Visible = false
Tooltip.ZIndex = 10
table.insert(shade1,Tooltip)

Title_3.Name = "Title"
Title_3.Parent = Tooltip
Title_3.BackgroundColor3 = Color3.fromRGB(46, 46, 47)
Title_3.BackgroundTransparency = 0.1
Title_3.BorderSizePixel = 0
Title_3.Size = UDim2.new(0, 200, 0, 20)
Title_3.Font = Enum.Font.SourceSans
Title_3.TextSize = 14
Title_3.Text = ""
Title_3.TextColor3 = Color3.new(1, 1, 1)
Title_3.TextTransparency = 0.1
Title_3.ZIndex = 10
table.insert(shade2,Title_3)
table.insert(text1,Title_3)

Description.Name = "Description"
Description.Parent = Tooltip
Description.BackgroundTransparency = 1
Description.BorderSizePixel = 0
Description.Size = UDim2.new(0,180,0,72)
Description.Position = UDim2.new(0,10,0,18)
Description.Font = Enum.Font.SourceSans
Description.TextSize = 16
Description.Text = ""
Description.TextColor3 = Color3.new(1, 1, 1)
Description.TextTransparency = 0.1
Description.TextWrapped = true
Description.ZIndex = 10
table.insert(text1,Description)

IntroBackground.Name = "IntroBackground"
IntroBackground.Parent = Holder
IntroBackground.Active = true
IntroBackground.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
IntroBackground.BorderSizePixel = 0
IntroBackground.Position = UDim2.new(0, 0, 0, 45)
IntroBackground.Size = UDim2.new(0, 250, 0, 175)
IntroBackground.ZIndex = 10

Logo.Name = "Logo"
Logo.Parent = Holder
Logo.BackgroundTransparency = 1
Logo.BorderSizePixel = 0
Logo.Position = UDim2.new(0, 125, 0, 127)
Logo.Size = UDim2.new(0, 10, 0, 10)
Logo.Image = "rbxassetid://1352543873"
Logo.ImageTransparency = 0
Logo.ZIndex = 10

Credits.Name = "Credits"
Credits.Parent = Holder
Credits.BackgroundTransparency = 1
Credits.BorderSizePixel = 0
Credits.Position = UDim2.new(0, 0, 0.9, 30)
Credits.Size = UDim2.new(0, 250, 0, 20)
Credits.Font = Enum.Font.SourceSansLight
Credits.FontSize = Enum.FontSize.Size18
Credits.Text = "Edge // Zwolf // Moon // Toon"
Credits.TextColor3 = Color3.new(1, 1, 1)
Credits.ZIndex = 10

KeybindsFrame.Name = "KeybindsFrame"
KeybindsFrame.Parent = Settings
KeybindsFrame.Active = true
KeybindsFrame.BackgroundColor3 = Color3.fromRGB(36, 36, 37)
KeybindsFrame.BorderSizePixel = 0
KeybindsFrame.Position = UDim2.new(0, 0, 0, 175)
KeybindsFrame.Size = UDim2.new(0, 250, 0, 175)
KeybindsFrame.ZIndex = 10
table.insert(shade1,KeybindsFrame)

Close.Name = "Close"
Close.Parent = KeybindsFrame
Cl
   end,
})

local Button = MainTab:CreateButton({
   Name = "TP gui",
   Callback = function()
   -- Gui to Lua
-- Version: 3.2

-- Instances:

local Tutorial = Instance.new("ScreenGui")
local OpenFrame = Instance.new("Frame")
local Open = Instance.new("TextButton")
local Main = Instance.new("Frame")
local TextLabel = Instance.new("TextLabel")
local TextLabel_2 = Instance.new("TextLabel")
local Close = Instance.new("TextButton")
local ImageLabel = Instance.new("ImageLabel")
local Teleport = Instance.new("TextButton")
local TextLabel_3 = Instance.new("TextLabel")
local TextBox = Instance.new("TextBox")

--Properties:

Tutorial.Name = "Tutorial"
Tutorial.Parent = game.CoreGui

OpenFrame.Name = "OpenFrame"
OpenFrame.Parent = Tutorial
OpenFrame.Active = true
OpenFrame.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
OpenFrame.BackgroundTransparency = 0.500
OpenFrame.BorderColor3 = Color3.fromRGB(0, 0, 0)
OpenFrame.Position = UDim2.new(0.891908348, 0, 0.654420495, 0)
OpenFrame.Size = UDim2.new(0, 100, 0, 50)

Open.Name = "Open"
Open.Parent = OpenFrame
Open.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Open.BackgroundTransparency = 0.500
Open.BorderColor3 = Color3.fromRGB(0, 0, 0)
Open.Position = UDim2.new(-0.000202026364, 0, -0.00305725099, 0)
Open.Size = UDim2.new(0, 100, 0, 50)
Open.Font = Enum.Font.Sarpanch
Open.Text = "Open"
Open.TextColor3 = Color3.fromRGB(255, 255, 255)
Open.TextScaled = true
Open.TextSize = 14.000
Open.TextStrokeColor3 = Color3.fromRGB(255, 255, 255)
Open.TextWrapped = true
Open.MouseButton1Down:connect(function()
	Main.Visible = true
	OpenFrame.Visible = false
end)

Main.Name = "Main"
Main.Parent = Tutorial
Main.Active = true
Main.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Main.BackgroundTransparency = 0.500
Main.BorderColor3 = Color3.fromRGB(0, 0, 0)
Main.Position = UDim2.new(0.206340134, 0, 0.291599989, 0)
Main.Size = UDim2.new(0, 583, 0, 332)
Main.Visible = false
Main.Draggable = true

TextLabel.Parent = Main
TextLabel.Active = true
TextLabel.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
TextLabel.BackgroundTransparency = 0.500
TextLabel.BorderColor3 = Color3.fromRGB(0, 0, 0)
TextLabel.Position = UDim2.new(0, 0, -0.00052341976, 0)
TextLabel.Size = UDim2.new(0, 583, 0, 50)
TextLabel.Font = Enum.Font.SourceSansItalic
TextLabel.Text = "Teleport Player GUI"
TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.TextScaled = true
TextLabel.TextSize = 14.000
TextLabel.TextStrokeColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.TextWrapped = true

TextLabel_2.Parent = Main
TextLabel_2.Active = true
TextLabel_2.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
TextLabel_2.BackgroundTransparency = 0.500
TextLabel_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
TextLabel_2.Position = UDim2.new(0, 0, 0.850090206, 0)
TextLabel_2.Size = UDim2.new(0, 583, 0, 50)
TextLabel_2.Font = Enum.Font.SourceSansItalic
TextLabel_2.Text = "GUI Maker : Ahmed_Prowy"
TextLabel_2.TextColor3 = Color3.fromRGB(255, 255, 255)
TextLabel_2.TextScaled = true
TextLabel_2.TextSize = 14.000
TextLabel_2.TextStrokeColor3 = Color3.fromRGB(255, 255, 255)
TextLabel_2.TextWrapped = true

Close.Name = "Close"
Close.Parent = Main
Close.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Close.BackgroundTransparency = 0.500
Close.BorderColor3 = Color3.fromRGB(0, 0, 0)
Close.Position = UDim2.new(0.914032459, 0, -0.000113993883, 0)
Close.Size = UDim2.new(0, 50, 0, 50)
Close.Font = Enum.Font.SourceSansSemibold
Close.Text = "X"
Close.TextColor3 = Color3.fromRGB(255, 255, 255)
Close.TextSize = 50.000
Close.TextStrokeColor3 = Color3.fromRGB(255, 255, 255)
Close.MouseButton1Down:connect(function()
	OpenFrame.Visible = true
	Main.Visible = false
end)

ImageLabel.Parent = Main
ImageLabel.Active = true
ImageLabel.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
ImageLabel.BackgroundTransparency = 1.000
ImageLabel.BorderColor3 = Color3.fromRGB(0, 0, 0)
ImageLabel.Position = UDim2.new(-5.47013187e-05, 0, -0.00138611393, 0)
ImageLabel.Size = UDim2.new(0, 75, 0, 50)
ImageLabel.Image = "http://www.roblox.com/asset/?id=6830485913"

Teleport.Name = "Teleport"
Teleport.Parent = Main
Teleport.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Teleport.BackgroundTransparency = 0.500
Teleport.BorderColor3 = Color3.fromRGB(0, 0, 0)
Teleport.Position = UDim2.new(0.217702299, 0, 0.640216887, 0)
Teleport.Size = UDim2.new(0, 328, 0, 49)
Teleport.Font = Enum.Font.Roboto
Teleport.Text = "Teleport"
Teleport.TextColor3 = Color3.fromRGB(255, 255, 255)
Teleport.TextSize = 40.000
Teleport.TextStrokeColor3 = Color3.fromRGB(255, 255, 255)
Teleport.TextWrapped = true
Teleport.MouseButton1Click:connect(function()
	local tp_namedplayer = TextBox.Text
	local tp_player = game:GetService("Players")[tp_namedplayer]
	local PLR = game:GetService("Players").LocalPlayer
	local p = TextBox.Text

	if tp_player then
		for i = 1,1 do
			wait(.08)
			PLR.Character.HumanoidRootPart.CFrame = tp_player.Character.HumanoidRootPart.CFrame + Vector3.new(0, 0, -1)
		end
	end
end)

TextLabel_3.Parent = Main
TextLabel_3.Active = true
TextLabel_3.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
TextLabel_3.BackgroundTransparency = 1.000
TextLabel_3.BorderColor3 = Color3.fromRGB(0, 0, 0)
TextLabel_3.Position = UDim2.new(0.106525294, 0, 0.148282975, 0)
TextLabel_3.Size = UDim2.new(0, 458, 0, 79)
TextLabel_3.Font = Enum.Font.Roboto
TextLabel_3.Text = "Enter The Players Name Here"
TextLabel_3.TextColor3 = Color3.fromRGB(255, 255, 255)
TextLabel_3.TextScaled = true
TextLabel_3.TextSize = 40.000
TextLabel_3.TextStrokeColor3 = Color3.fromRGB(255, 255, 255)
TextLabel_3.TextWrapped = true

TextBox.Parent = Main
TextBox.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextBox.BackgroundTransparency = 0.700
TextBox.Position = UDim2.new(0.217702314, 0, 0.423602074, 0)
TextBox.Size = UDim2.new(0, 329, 0, 50)
TextBox.Font = Enum.Font.Roboto
TextBox.Text = "Player"
TextBox.TextColor3 = Color3.fromRGB(0, 0, 0)
TextBox.TextSize = 40.000
   end,
})
