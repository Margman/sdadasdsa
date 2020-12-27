--[[
	 Gui to Lua Converter
-- Revamped by:HoIyScript
--]]



-- Instances:

local ScreenGui = Instance.new("ScreenGui")
local Main = Instance.new("Frame")
local message = Instance.new("TextBox")
local spam = Instance.new("TextButton")

--[[
	Properties:
--]]

ScreenGui.Parent = game.CoreGui
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

Main.Name = "Main"
Main.Parent = ScreenGui
Main.BackgroundColor3 = Color3.new(0.666667, 0.666667, 1)
Main.Position = UDim2.new(0.724363625, 0, 0.643734634, 0)
Main.Size = UDim2.new(0, 327, 0, 247)

message.Name = "message"
message.Parent = Main
message.BackgroundColor3 = Color3.new(1, 1, 1)
message.Position = UDim2.new(0.220183492, 0, 0, 0)
message.Size = UDim2.new(0, 188, 0, 34)
message.PlaceholderColor3 = Color3.new(0, 0, 0.498039)
message.Text = "message"
message.TextColor3 = Color3.new(0, 0, 0)
message.TextSize = 14

spam.Name = "spam"
spam.Parent = Main
spam.BackgroundColor3 = Color3.new(1, 1, 1)
spam.Position = UDim2.new(0.287461787, 0, 0.178137645, 0)
spam.Size = UDim2.new(0, 149, 0, 32)
spam.Font = Enum.Font.Fantasy
spam.Text = "send!"
spam.TextColor3 = Color3.new(0, 0, 0)
spam.TextSize = 30

local p = game.Players.localPlayer
local mouse = p:GetMouse()
mouse.KeyDown:connect(function(key)
if key == "q" then
		Main.Visible = false
	elseif
		Main.Visible == false then
		Main.Visible = true
	
		end
end)

spam.MouseButton1Down:Connect(function()
	game:GetService"ReplicatedStorage".DefaultChatSystemChatEvents.SayMessageRequest:FireServer(message.Text ,"All")
	wait(3)
	game:GetService"ReplicatedStorage".DefaultChatSystemChatEvents.SayMessageRequest:FireServer(message.Text ,"All")
	wait(3)
	game:GetService"ReplicatedStorage".DefaultChatSystemChatEvents.SayMessageRequest:FireServer(message.Text ,"All")
	wait(3)
	game:GetService"ReplicatedStorage".DefaultChatSystemChatEvents.SayMessageRequest:FireServer(message.Text ,"All")
	wait(3)
	game:GetService"ReplicatedStorage".DefaultChatSystemChatEvents.SayMessageRequest:FireServer(message.Text ,"All")
	wait(3)
	game:GetService"ReplicatedStorage".DefaultChatSystemChatEvents.SayMessageRequest:FireServer(message.Text ,"All")
	wait(3)
	game:GetService"ReplicatedStorage".DefaultChatSystemChatEvents.SayMessageRequest:FireServer(message.Text ,"All")
	wait(3)
	game:GetService"ReplicatedStorage".DefaultChatSystemChatEvents.SayMessageRequest:FireServer(message.Text ,"All")
 end)
