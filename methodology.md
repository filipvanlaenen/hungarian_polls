# Methodology

## Confidence Intervals

## Weighted Monte Carlo Simulations

## Projecting National Results on Electoral Districts

Opinion polls usually only give data on a national level. Unless there is only
one, national electoral district, these data have to be translated to the local
electoral districts one way or the other. The model used to produce the numbers
on these pages is a variant of the so-called uniform regional swing, which means
that it projects the national tendencies onto the local electorale districts
without any adjustments.

### Multiplicative Uniform Regional Swing

Assume that a party had a voting share of 20 percent at the last election,
but that an opinion poll shows that the voting intentions for the party have
risen to 22 percent. One way to project this change onto the local electoral
districts, is to take the last election result in every electoral district, and
simply add the national change to each of them. This means that if the party
scored 25 percent in a particular district, the new score used to calculate the
number of seats in that district will be 25 + 2 = 27. If the party had voting
share of only 15 percent, the new score would be 15 + 2 = 17 percent.

This model works fine for parties increasing their result, and parties with a
modest to large vote share across all electoral district. However, for small
parties losing votes, the model can result into negative numbers in the
electoral districts where it performed poorely during the last election. Just
imagine a party going from 8 to 5 percent nationally, but with a local score
of only 2 percent in one of the electoral districts. The uniform regional
swing mode described above would project the party at 2 - 3 = -1 percent in
that district.

As an alternative, the model used on these pages projects the national results
onto the local districts in a multiplicative way. That means that when a party
increases from 20 to 22 percent, the model doesn't add 2 percent to the party's
voting share in every district, but *multiplies* the local results with a factor
of 22 / 20 = 1.1. In the example mentioned above, this would put the party in
the district where it score 25 percent last time at 27.5 percent, and in the
district where it scored only 15 percent at 16.5 percent. For the party losing
votes, the factor would be 5 / 8 = 0.625, thus projecting the party in the
district where it score 2 percent last time at 1.25 percent.

Is multiplicative uniform regional swing more correct than additive uniform
regional swing? Hard to say. Multiplicative uniform regional swing will make
parties swing more in electoral districts where they had a high score at the
last election. For parties gaining support, that may be incorrect, if they are
gaining more national support because they're mainly getting more support in
those districts where they performed less during the last election. But it's
easy to produce counterexamples where a multiplicative approach will be more
correct than the additive.

As a general rule, using multiplicative or additive uniform regional swing
should not make much of a difference for seat projections on the national
level. Overestimations in one electoral districts will often be compensated by
underestimations in other electoral districts, such that the overall result
will be more or less correct. Remember that in the end, a party gaining support
on a national level may very well be losing votes in some parts of the country.
The projection of the national results onto the local electoral districts
should therefore not be used to predict local results, but only as a way to
calculate national seat projections. If you want to know how a party is doing
locally, the best way to find out about this is to run a local opinion poll.

### Regional Data

From time to time, pollsters will run local opinion polls, or publish regional
tendencies in their national polls. Advanced models could use this information
in order to project national polling results more accurately onto local
electoral districs. In some occassions, e.g. when there are parties with a
particular local stronghold, this may give more accurate results on a national
level. On the other hand, if these local results give better results on a
national, it would probably be wiser not to project the national results onto
those local electoral districts, and instead just use the regional data
directly.

### Historic Data

Some models try and use more of the historic data in every electoral district.
But in Western countries, with election cycles of four or five years, this means
that models use data that is eight to ten years old if last two elections are
used, and twelve to fifteen years old if three elections are used. It is
questionable how relevant such historic data can be with new parties emerging,
old parties disappearing, in addition to changing demographics. Sometimes, even
using data from the last election, which may not be older than three or four
years, seems hopeless because of deep changes in national politics.

### Incumbency

Some studies have shown that incumbent candidates have a slight advantage over
their opponents. However, when trying to calculate national results, incumbency
should make a difference, since any significant change would already have been
included in the national polling results. Therefore, incumbency has not been
modeled in for the calculation of the numbers presented on these pages.

### House Factors and Other Corrective Measures

Some modelers try to improve the raw polling results using "house factors".
Basically, these house factors try to compensate for the historic errors
pollsters have made, e.g. if they have consistently underestimated a party with
a certain percentage. Others also include economic or demographic data, e.g.
giving a slight advantage to the parties in government if the economy is doing
well, or vice versa.

House factors may work to a certain degree in countries with a bipartisan
political landscape, but they quickly break down when there are many parties
involved, or when there are large or even disruptive changes. Furthermore,
for obvious reasons, house factors won't work for new parties.

The numbers presented on these pages try to explain in more detail the true
meaning of opinion polling results. Therefore, the model doesn't try to
"improve" any opinion polling result with house factors or other parameters.

As a personal note, it is also my belief that pollsters have a large interest in
trying to get their opinion polling results as correct as possible, and
therefore will have a huge incentive to learn from theire mistakes. House
factors seem therefore a bit patronizing.

### New Parties

Since the method described above relies on regional data in order to calculate
the number of seats in parliament, new parties that haven't participated in the
previous election pose a probleme. However, there are number of strategies that
can be used to estimate the regional distribution of the new party's voters:

* If party A and party B merge together to form a new party C, the regional data
  for the parties A and B can simply added together as an estimate for the new
  party's, even though we know that in politics, 1 + 1 ⋚ 2.
* If a dissidency in a party A breaks out and forms a new party B, the regional
  data for party A can simply be divided equally between the old party A and the
  new party B. Multiplicative uniform regional swing will then scale both
  parties up or down in all electoral districts, but the size of the parties
  will off course be the same in all electoral districts.
* In case an entirely new party has been created, the best estimate will
  probably be the assumption of a uniform distribution across the entire
  country. This can be achieved by setting the party's size equal to e.g. one
  percent of the population in each electoral district. Again, multiplicative
  uniform swing will then scale the party up or down in all electoral districts,
  in accordance with the party's result in the poll.

Note however that in the case where more information is known about the newly
formed party, it is always wise to include it. If it's e.g. known that the new
party will only participate in the election in a part of the country, the
regional data for the new party should be adjusted in that way.

## Holes and Spikes in Probability Mass Functions

## Calculation of the Error Estimate
