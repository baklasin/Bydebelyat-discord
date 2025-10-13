Я одинокий русский писатель скриптов и хочу получить поддержку так как не требую не ключа и делаю качественные скрипты



Если у вас неработает авто покупка то зайдите в скрипт и найдите код ниже
 
task.spawn(function()
	local event = ReplicatedStorage.Shared.Remotes.ShopRemotes:WaitForChild("BuyGacha")
	while task.wait(0.2) do
		if autoClick then
			-- Сначала x50
			event:FireServer("x50")
			task.wait(0.1)
			-- Потом 10
			event:FireServer("10")
		end
	end
end)

после замените всю строчку кода на код ниже

while task.wait(0.2) do
	if autoClick then
		event:FireServer("x50") -- в этой строчке у вас должно быть сколько вы хотите покупать за раз есть 3 варианта 1 - 10 и 50 но 50 только с геймпассом
 	end
end

после чего у вас должно сработать
