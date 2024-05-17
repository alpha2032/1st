# 1st
# FOR SIMPLE INTEREST 
puts "Enter principal amount:" 
p = Integer(gets.chomp) 
puts "Enter number of years:" 
t = Integer(gets.chomp) 
puts "Enter rate of interest:" 
r = Float(gets.chomp) 
i = 1 
while i <= t 
interest = p * r * i * 0.01 
puts "The simple interest for year #{i} is #{interest}" 
i += 1 
end 
# FOR COMPOUND INTEREST 
puts "Enter principal amount:" 
p = Integer(gets.chomp) 
puts "Enter number of years:" 
t = Integer(gets.chomp) 
puts "Enter rate of interest:" 
r = Float(gets.chomp) 
i = 1 
while i <= t 
interest = p * ((1 + r / 100) ** i - 1) 
puts "The compound interest for year #{i} is #{interest}" 
p += interest 
i += 1 
end 
