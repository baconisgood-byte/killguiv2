-- GUI with a Close button
local Players = game:GetService("Players")
local player = Players.LocalPlayer
local playerGui = player:WaitForChild("PlayerGui")

-- Remove old GUI if it exists
local oldGui = playerGui:FindFirstChild("MyGui")
if oldGui then
    oldGui:Destroy()
end

-- Create ScreenGui
local screenGui = Instance.new("ScreenGui")
screenGui.Name = "MyGui"
screenGui.Parent = playerGui

-- Main Frame
local frame = Instance.new("Frame")
frame.Size = UDim2.new(0, 250, 0, 150)
frame.Position = UDim2.new(0.5, -125, 0.5, -75)
frame.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
frame.Parent = screenGui

-- Label
local label = Instance.new("TextLabel")
label.Size = UDim2.new(1, 0, 0.6, 0)
label.BackgroundTransparency = 1
label.Text = "Hello!"
label.TextColor3 = Color3.fromRGB(255, 255, 255)
label.TextScaled = true
label.Parent = frame

-- Close Button
local closeButton = Instance.new("TextButton")
closeButton.Size = UDim2.new(0.3, 0, 0.3, 0)
closeButton.Position = UDim2.new(0.35, 0, 0.65, 0)
closeButton.BackgroundColor3 = Color3.fromRGB(200, 0, 0)
closeButton.Text = "Close"
closeButton.TextColor3 = Color3.fromRGB(255, 255, 255)
closeButton.TextScaled = true
closeButton.Parent = frame

closeButton.MouseButton1Click:Connect(function()
    screenGui:Destroy()
end)
