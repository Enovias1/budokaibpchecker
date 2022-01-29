-- Gui to Lua
-- Version: 3.2

-- Instances:

local BpChecker = Instance.new("ScreenGui")
local Frame3090 = Instance.new("Frame")
local UICorner = Instance.new("UICorner")
local BP = Instance.new("TextLabel")

--Properties:

BpChecker.Name = "BpChecker"
BpChecker.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
BpChecker.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
BpChecker.ResetOnSpawn = false

Frame3090.Name = "Frame3090"
Frame3090.Parent = BpChecker
Frame3090.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Frame3090.BackgroundTransparency = 0.300
Frame3090.BorderSizePixel = 0
Frame3090.Position = UDim2.new(0.218315035, 0, 0.334446013, 0)
Frame3090.Size = UDim2.new(0, 217, 0, 24)

UICorner.Parent = Frame3090

BP.Name = "BP"
BP.Parent = Frame3090
BP.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
BP.BackgroundTransparency = 1.000
BP.Size = UDim2.new(0, 217, 0, 24)
BP.Font = Enum.Font.SourceSans
BP.TextColor3 = Color3.fromRGB(0, 0, 0)
BP.TextSize = 14.000

local function WZYDOYK_fake_script() -- BPShitText.BPShitScript
    local script = Instance.new('LocalScript', BP)

    while wait(1) do
        script.Parent.Text = "BattlePower: "..game.Players.LocalPlayer.Character.StandardValues.BattlePower.Value --
    end
end
coroutine.wrap(WZYDOYK_fake_script)()

local gui = game:GetService("Players").LocalPlayer.PlayerGui.BpChecker
local frame = gui:FindFirstChild("Frame3090")
frame.Active = true
frame.Draggable = true
