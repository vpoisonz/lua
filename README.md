CREDITS TO: FRESA N SWIFTIE
-----
JOIN AND LEAVES SCRIPT

-- player joins and leaves the server

local Players = game:GetService("Players")

--
local function showNotification(message)
    game.StarterGui:SetCore("SendNotification", {
        Title = "by: swiftie";
        Text = message;
        Duration = 5;
    })
end

--
Players.PlayerAdded:Connect(function(player)
    showNotification(player.Name .. " Nigga join the server.")
end)

--
Players.PlayerRemoving:Connect(function(player)
    showNotification(player.Name .. " Nigga leave the server.")
end)
