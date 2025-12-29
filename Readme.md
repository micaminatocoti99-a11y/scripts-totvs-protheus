# Script para TOTVS Microsiga Protheus 

Script utilizado para facilitar e automatizar algumas operações diárias. 
-- LocalScript (S)

local player = game.Players.LocalPlayer

player.CharacterAdded:Connect(function(char)
	local hrp = char:WaitForChild("HumanoidRootPart")

	local box = Instance.new("BoxHandleAdornment")
	box.Size = Vector3.new(6, 6, 6) -- visual maior
	box.Color3 = Color3.fromRGB(0, 255, 0)
	box.Transparency = 0.7
	box.AlwaysOnTop = true
	box.Adornee = hrp
	box.Parent = hrp
end)
