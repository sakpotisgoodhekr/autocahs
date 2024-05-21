local player = game.Players.LocalPlayer

-- Function to add cash to the player
local function addCash()
    while true do
        local cash = player.leaderstats:FindFirstChild("Cash")
        if cash then
            cash.Value = cash.Value + 1000
        end
        wait(1) -- Wait for 1 second before adding cash again
    end
end

-- Start adding cash
addCash()
