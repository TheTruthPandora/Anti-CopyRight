local TeleportService = game:GetService("TeleportService")
local targetPlaceId = 14296228821 -- 要传送到的游戏的PlaceId

wait(5)

if game.PlaceId ~= targetPlaceId then
    for _, player in ipairs(game.Players:GetPlayers()) do
				player:Kick("ANTI COPYRIGHT")
		wait(.35)
        TeleportService:Teleport(targetPlaceId, player) -- 将玩家传送到目标游戏
    end
end
