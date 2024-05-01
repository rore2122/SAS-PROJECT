filename ODI "/home/u63815565/odi2023.csv";
data ODI;
length player $50 Runs $10 Mins $10 Balls $10 fours 8 sixes 8  SR $10 Team $50 Oponent $50 Ground $50;
infile ODI dsd dlm=',' missover;
input player $ Runs $ Mins Balls fours sixes SR $ Team $ Oponent $ Ground $;
run;
