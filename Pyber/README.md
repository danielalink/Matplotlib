

```python
#import libraries
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

#sns.factorplot
#lmplot, pointplot
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>city</th>
      <th>driver_count</th>
      <th>type</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Richardfort</td>
      <td>38</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Williamsstad</td>
      <td>59</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Port Angela</td>
      <td>67</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Rodneyfort</td>
      <td>34</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>4</th>
      <td>West Robert</td>
      <td>39</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>5</th>
      <td>West Anthony</td>
      <td>70</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>6</th>
      <td>West Angela</td>
      <td>48</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Martinezhaven</td>
      <td>25</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Karenberg</td>
      <td>22</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Barajasview</td>
      <td>26</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>10</th>
      <td>Robertport</td>
      <td>12</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>11</th>
      <td>Joneschester</td>
      <td>39</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>12</th>
      <td>Leahton</td>
      <td>17</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>13</th>
      <td>West Christopherberg</td>
      <td>32</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>14</th>
      <td>Johnton</td>
      <td>27</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>15</th>
      <td>Reynoldsfurt</td>
      <td>67</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>16</th>
      <td>Port David</td>
      <td>7</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>17</th>
      <td>New Kimberlyborough</td>
      <td>33</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>18</th>
      <td>Carriemouth</td>
      <td>52</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>19</th>
      <td>Rogerston</td>
      <td>25</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>20</th>
      <td>Jerryton</td>
      <td>64</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>21</th>
      <td>Loganberg</td>
      <td>23</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>22</th>
      <td>Simpsonburgh</td>
      <td>21</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>23</th>
      <td>Port Frank</td>
      <td>23</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>24</th>
      <td>South Latoya</td>
      <td>10</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>25</th>
      <td>West Samuelburgh</td>
      <td>73</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>26</th>
      <td>Grahamburgh</td>
      <td>61</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>27</th>
      <td>West Patrickchester</td>
      <td>25</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>28</th>
      <td>North Madeline</td>
      <td>19</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>29</th>
      <td>South Jack</td>
      <td>46</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>90</th>
      <td>Barronchester</td>
      <td>11</td>
      <td>Suburban</td>
    </tr>
    <tr>
      <th>91</th>
      <td>Brandonfort</td>
      <td>10</td>
      <td>Suburban</td>
    </tr>
    <tr>
      <th>92</th>
      <td>East Danielview</td>
      <td>22</td>
      <td>Suburban</td>
    </tr>
    <tr>
      <th>93</th>
      <td>East Marymouth</td>
      <td>5</td>
      <td>Suburban</td>
    </tr>
    <tr>
      <th>94</th>
      <td>Mezachester</td>
      <td>14</td>
      <td>Suburban</td>
    </tr>
    <tr>
      <th>95</th>
      <td>Lewisland</td>
      <td>4</td>
      <td>Suburban</td>
    </tr>
    <tr>
      <th>96</th>
      <td>Josephside</td>
      <td>25</td>
      <td>Suburban</td>
    </tr>
    <tr>
      <th>97</th>
      <td>Davidfurt</td>
      <td>23</td>
      <td>Suburban</td>
    </tr>
    <tr>
      <th>98</th>
      <td>Nicolechester</td>
      <td>19</td>
      <td>Suburban</td>
    </tr>
    <tr>
      <th>99</th>
      <td>East Aaronbury</td>
      <td>7</td>
      <td>Suburban</td>
    </tr>
    <tr>
      <th>100</th>
      <td>North Richardhaven</td>
      <td>1</td>
      <td>Suburban</td>
    </tr>
    <tr>
      <th>101</th>
      <td>North Jeffrey</td>
      <td>11</td>
      <td>Suburban</td>
    </tr>
    <tr>
      <th>102</th>
      <td>South Jennifer</td>
      <td>7</td>
      <td>Rural</td>
    </tr>
    <tr>
      <th>103</th>
      <td>West Heather</td>
      <td>4</td>
      <td>Rural</td>
    </tr>
    <tr>
      <th>104</th>
      <td>Newtonview</td>
      <td>1</td>
      <td>Rural</td>
    </tr>
    <tr>
      <th>105</th>
      <td>North Holly</td>
      <td>8</td>
      <td>Rural</td>
    </tr>
    <tr>
      <th>106</th>
      <td>Michaelberg</td>
      <td>6</td>
      <td>Rural</td>
    </tr>
    <tr>
      <th>107</th>
      <td>Taylorhaven</td>
      <td>1</td>
      <td>Rural</td>
    </tr>
    <tr>
      <th>108</th>
      <td>Penaborough</td>
      <td>6</td>
      <td>Rural</td>
    </tr>
    <tr>
      <th>109</th>
      <td>Harringtonfort</td>
      <td>4</td>
      <td>Rural</td>
    </tr>
    <tr>
      <th>110</th>
      <td>Lake Jamie</td>
      <td>4</td>
      <td>Rural</td>
    </tr>
    <tr>
      <th>111</th>
      <td>Lake Latoyabury</td>
      <td>2</td>
      <td>Rural</td>
    </tr>
    <tr>
      <th>112</th>
      <td>North Jaime</td>
      <td>1</td>
      <td>Rural</td>
    </tr>
    <tr>
      <th>113</th>
      <td>South Marychester</td>
      <td>1</td>
      <td>Rural</td>
    </tr>
    <tr>
      <th>114</th>
      <td>Garzaport</td>
      <td>7</td>
      <td>Rural</td>
    </tr>
    <tr>
      <th>115</th>
      <td>Bradshawfurt</td>
      <td>7</td>
      <td>Rural</td>
    </tr>
    <tr>
      <th>116</th>
      <td>New Ryantown</td>
      <td>2</td>
      <td>Rural</td>
    </tr>
    <tr>
      <th>117</th>
      <td>Randallchester</td>
      <td>9</td>
      <td>Rural</td>
    </tr>
    <tr>
      <th>118</th>
      <td>Jessicaport</td>
      <td>1</td>
      <td>Rural</td>
    </tr>
    <tr>
      <th>119</th>
      <td>South Saramouth</td>
      <td>7</td>
      <td>Rural</td>
    </tr>
  </tbody>
</table>
<p>120 rows × 3 columns</p>
</div>




```python
data_city = pd.read_csv("raw_data/city_data.csv")
data_ride = pd.read_csv("raw_data/ride_data.csv")
data = data_ride.merge(data_city, on="city",how="left")
data.head(5)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>city</th>
      <th>date</th>
      <th>fare</th>
      <th>ride_id</th>
      <th>driver_count</th>
      <th>type</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Lake Jonathanshire</td>
      <td>2018-01-14 10:14:22</td>
      <td>13.83</td>
      <td>5739410935873</td>
      <td>5</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>1</th>
      <td>South Michelleport</td>
      <td>2018-03-04 18:24:09</td>
      <td>30.24</td>
      <td>2343912425577</td>
      <td>72</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Port Samanthamouth</td>
      <td>2018-02-24 04:29:00</td>
      <td>33.44</td>
      <td>2005065760003</td>
      <td>57</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Rodneyfort</td>
      <td>2018-02-10 23:22:03</td>
      <td>23.44</td>
      <td>5149245426178</td>
      <td>34</td>
      <td>Urban</td>
    </tr>
    <tr>
      <th>4</th>
      <td>South Jack</td>
      <td>2018-03-06 04:28:35</td>
      <td>34.58</td>
      <td>3908451377344</td>
      <td>46</td>
      <td>Urban</td>
    </tr>
  </tbody>
</table>
</div>




```python
#pull data from table
groupby_city = data.groupby("city")
average_fare = groupby_city["fare"].mean()
total_rides = groupby_city["ride_id"].count()
driver_count = data_city.set_index("city")["driver_count"]
city_type = data_city.set_index("city")["type"]
summary = pd.DataFrame({"average_fare":average_fare,"total_rides":total_rides,"driver_count":driver_count,"city_type":city_type})
groupby_type = summary.groupby("city_type")
summary
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>average_fare</th>
      <th>city_type</th>
      <th>driver_count</th>
      <th>total_rides</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Amandaburgh</th>
      <td>24.641667</td>
      <td>Urban</td>
      <td>12</td>
      <td>18</td>
    </tr>
    <tr>
      <th>Barajasview</th>
      <td>25.332273</td>
      <td>Urban</td>
      <td>26</td>
      <td>22</td>
    </tr>
    <tr>
      <th>Barronchester</th>
      <td>36.422500</td>
      <td>Suburban</td>
      <td>11</td>
      <td>16</td>
    </tr>
    <tr>
      <th>Bethanyland</th>
      <td>32.956111</td>
      <td>Suburban</td>
      <td>22</td>
      <td>18</td>
    </tr>
    <tr>
      <th>Bradshawfurt</th>
      <td>40.064000</td>
      <td>Rural</td>
      <td>7</td>
      <td>10</td>
    </tr>
    <tr>
      <th>Brandonfort</th>
      <td>35.437368</td>
      <td>Suburban</td>
      <td>10</td>
      <td>19</td>
    </tr>
    <tr>
      <th>Carriemouth</th>
      <td>28.314444</td>
      <td>Urban</td>
      <td>52</td>
      <td>27</td>
    </tr>
    <tr>
      <th>Christopherfurt</th>
      <td>24.501852</td>
      <td>Urban</td>
      <td>41</td>
      <td>27</td>
    </tr>
    <tr>
      <th>Colemanland</th>
      <td>30.894545</td>
      <td>Suburban</td>
      <td>23</td>
      <td>22</td>
    </tr>
    <tr>
      <th>Davidfurt</th>
      <td>31.995882</td>
      <td>Suburban</td>
      <td>23</td>
      <td>17</td>
    </tr>
    <tr>
      <th>Deanville</th>
      <td>25.842632</td>
      <td>Urban</td>
      <td>49</td>
      <td>19</td>
    </tr>
    <tr>
      <th>East Aaronbury</th>
      <td>25.661111</td>
      <td>Suburban</td>
      <td>7</td>
      <td>9</td>
    </tr>
    <tr>
      <th>East Danielview</th>
      <td>31.560588</td>
      <td>Suburban</td>
      <td>22</td>
      <td>17</td>
    </tr>
    <tr>
      <th>East Kaylahaven</th>
      <td>23.757931</td>
      <td>Urban</td>
      <td>65</td>
      <td>29</td>
    </tr>
    <tr>
      <th>East Kentstad</th>
      <td>29.823077</td>
      <td>Suburban</td>
      <td>20</td>
      <td>13</td>
    </tr>
    <tr>
      <th>East Marymouth</th>
      <td>30.835185</td>
      <td>Suburban</td>
      <td>5</td>
      <td>27</td>
    </tr>
    <tr>
      <th>Erikaland</th>
      <td>24.906667</td>
      <td>Urban</td>
      <td>37</td>
      <td>12</td>
    </tr>
    <tr>
      <th>Garzaport</th>
      <td>24.123333</td>
      <td>Rural</td>
      <td>7</td>
      <td>3</td>
    </tr>
    <tr>
      <th>Grahamburgh</th>
      <td>25.221200</td>
      <td>Urban</td>
      <td>61</td>
      <td>25</td>
    </tr>
    <tr>
      <th>Grayville</th>
      <td>27.763333</td>
      <td>Suburban</td>
      <td>2</td>
      <td>15</td>
    </tr>
    <tr>
      <th>Harringtonfort</th>
      <td>33.470000</td>
      <td>Rural</td>
      <td>4</td>
      <td>6</td>
    </tr>
    <tr>
      <th>Huntermouth</th>
      <td>28.993750</td>
      <td>Urban</td>
      <td>37</td>
      <td>24</td>
    </tr>
    <tr>
      <th>Hurleymouth</th>
      <td>25.891429</td>
      <td>Urban</td>
      <td>36</td>
      <td>28</td>
    </tr>
    <tr>
      <th>Jerryton</th>
      <td>25.649200</td>
      <td>Urban</td>
      <td>64</td>
      <td>25</td>
    </tr>
    <tr>
      <th>Jessicaport</th>
      <td>36.013333</td>
      <td>Rural</td>
      <td>1</td>
      <td>6</td>
    </tr>
    <tr>
      <th>Johnton</th>
      <td>26.785714</td>
      <td>Urban</td>
      <td>27</td>
      <td>21</td>
    </tr>
    <tr>
      <th>Joneschester</th>
      <td>22.289600</td>
      <td>Urban</td>
      <td>39</td>
      <td>25</td>
    </tr>
    <tr>
      <th>Josephside</th>
      <td>32.858148</td>
      <td>Suburban</td>
      <td>25</td>
      <td>27</td>
    </tr>
    <tr>
      <th>Justinberg</th>
      <td>23.694333</td>
      <td>Urban</td>
      <td>39</td>
      <td>30</td>
    </tr>
    <tr>
      <th>Karenberg</th>
      <td>26.340000</td>
      <td>Urban</td>
      <td>22</td>
      <td>17</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>South Evanton</th>
      <td>26.726129</td>
      <td>Urban</td>
      <td>11</td>
      <td>31</td>
    </tr>
    <tr>
      <th>South Jack</th>
      <td>22.965263</td>
      <td>Urban</td>
      <td>46</td>
      <td>19</td>
    </tr>
    <tr>
      <th>South Jennifer</th>
      <td>35.264286</td>
      <td>Rural</td>
      <td>7</td>
      <td>7</td>
    </tr>
    <tr>
      <th>South Karenland</th>
      <td>26.535526</td>
      <td>Urban</td>
      <td>4</td>
      <td>38</td>
    </tr>
    <tr>
      <th>South Latoya</th>
      <td>20.093158</td>
      <td>Urban</td>
      <td>10</td>
      <td>19</td>
    </tr>
    <tr>
      <th>South Marychester</th>
      <td>41.870000</td>
      <td>Rural</td>
      <td>1</td>
      <td>8</td>
    </tr>
    <tr>
      <th>South Michelleport</th>
      <td>24.451613</td>
      <td>Urban</td>
      <td>72</td>
      <td>31</td>
    </tr>
    <tr>
      <th>South Phillip</th>
      <td>28.571290</td>
      <td>Urban</td>
      <td>38</td>
      <td>31</td>
    </tr>
    <tr>
      <th>South Saramouth</th>
      <td>36.160000</td>
      <td>Rural</td>
      <td>7</td>
      <td>4</td>
    </tr>
    <tr>
      <th>South Teresa</th>
      <td>31.220455</td>
      <td>Suburban</td>
      <td>21</td>
      <td>22</td>
    </tr>
    <tr>
      <th>Taylorhaven</th>
      <td>42.263333</td>
      <td>Rural</td>
      <td>1</td>
      <td>6</td>
    </tr>
    <tr>
      <th>Valentineton</th>
      <td>24.636364</td>
      <td>Urban</td>
      <td>45</td>
      <td>22</td>
    </tr>
    <tr>
      <th>Veronicaberg</th>
      <td>32.828235</td>
      <td>Suburban</td>
      <td>20</td>
      <td>17</td>
    </tr>
    <tr>
      <th>Victoriaport</th>
      <td>27.780000</td>
      <td>Suburban</td>
      <td>16</td>
      <td>14</td>
    </tr>
    <tr>
      <th>West Angela</th>
      <td>25.990000</td>
      <td>Urban</td>
      <td>48</td>
      <td>39</td>
    </tr>
    <tr>
      <th>West Anthony</th>
      <td>24.736667</td>
      <td>Urban</td>
      <td>70</td>
      <td>30</td>
    </tr>
    <tr>
      <th>West Christopherberg</th>
      <td>24.421154</td>
      <td>Urban</td>
      <td>32</td>
      <td>26</td>
    </tr>
    <tr>
      <th>West Ericstad</th>
      <td>22.347222</td>
      <td>Urban</td>
      <td>25</td>
      <td>18</td>
    </tr>
    <tr>
      <th>West Gabriel</th>
      <td>20.346087</td>
      <td>Urban</td>
      <td>57</td>
      <td>23</td>
    </tr>
    <tr>
      <th>West Hannah</th>
      <td>29.547619</td>
      <td>Suburban</td>
      <td>12</td>
      <td>21</td>
    </tr>
    <tr>
      <th>West Heather</th>
      <td>33.890000</td>
      <td>Rural</td>
      <td>4</td>
      <td>9</td>
    </tr>
    <tr>
      <th>West Heidi</th>
      <td>23.133929</td>
      <td>Urban</td>
      <td>28</td>
      <td>28</td>
    </tr>
    <tr>
      <th>West Josephberg</th>
      <td>21.720385</td>
      <td>Urban</td>
      <td>45</td>
      <td>26</td>
    </tr>
    <tr>
      <th>West Kimmouth</th>
      <td>29.871500</td>
      <td>Suburban</td>
      <td>4</td>
      <td>20</td>
    </tr>
    <tr>
      <th>West Patrickchester</th>
      <td>28.233125</td>
      <td>Urban</td>
      <td>25</td>
      <td>16</td>
    </tr>
    <tr>
      <th>West Robert</th>
      <td>25.123871</td>
      <td>Urban</td>
      <td>39</td>
      <td>31</td>
    </tr>
    <tr>
      <th>West Samuelburgh</th>
      <td>21.767600</td>
      <td>Urban</td>
      <td>73</td>
      <td>25</td>
    </tr>
    <tr>
      <th>Williamsonville</th>
      <td>31.875000</td>
      <td>Suburban</td>
      <td>2</td>
      <td>14</td>
    </tr>
    <tr>
      <th>Williamsstad</th>
      <td>24.362174</td>
      <td>Urban</td>
      <td>59</td>
      <td>23</td>
    </tr>
    <tr>
      <th>Williamsview</th>
      <td>26.599000</td>
      <td>Urban</td>
      <td>46</td>
      <td>20</td>
    </tr>
  </tbody>
</table>
<p>120 rows × 4 columns</p>
</div>




```python
#build plot
g = sns.lmplot(x= "total_rides",
               y = "average_fare",
               data=summary,
               palette={'Rural': 'gold', 'Suburban': 'lightskyblue', 'Urban': 'lightcoral'},
               hue="city_type",
               size = 10,
               aspect = 1.5,
               fit_reg=False,
               legend=False,
                   scatter_kws={'s':summary["driver_count"]*100,
                                'alpha':0.5,
                                'linewidth':2}
              )
ax = g.ax
ax.text(42,27,'Note: \nCircle size correlates with \ndriver count per city.').set_fontsize(30)
ax.legend(loc='upper right', fontsize=35, markerscale=.5, frameon=False)
ax.set_title('Pyber Ride Sharing Data (2018)').set_fontsize(40)
ax.set_xlabel('Total Number of Rides (Per City)').set_fontsize(30)
ax.set_ylabel('Average Fare ($)').set_fontsize(30)
ax.tick_params(which='major', labelsize=25)
ax.set_facecolor('white')
ax.grid(color='grey',linestyle='-',linewidth= 1,alpha = 0.1)
g.savefig('bubble.png')
```


![png](output_3_0.png)



```python
data_group = data.groupby(by='type',as_index=True)

type_index = list(type_fare.index)
type_fare = data_group['fare'].sum()
plt.pie(type_fare,explode = (0.1,0,0), labels = type_index, colors = ['gold', 'lightskyblue', 'lightcoral'],autopct="%1.1f%%",
       shadow = True, startangle = 40)
plt.axis('equal')
plt.title('% of Total Fares by City Type')
plt.savefig('fare by city type.png')
```


![png](output_4_0.png)



```python
type_index = list(type_fare.index)
type_ride = data_group.size()
plt.pie(type_ride,explode = (0.1,0,0), labels = type_index, colors = ['gold', 'lightskyblue', 'lightcoral'],autopct="%1.1f%%",
       shadow = True, startangle = 40)
plt.axis('equal')
plt.title('% of Total Rides by City Type')
plt.savefig('ride by city type.png')
```


![png](output_5_0.png)



```python
city_group = data_city.groupby('type')

type_index = list(type_fare.index)
type_drivers = city_group['driver_count'].sum()
plt.pie(type_drivers,explode = (0.1,0,0), labels = type_index, colors = ['gold', 'lightskyblue', 'lightcoral'],autopct="%1.1f%%",
       shadow = True, startangle = 40)
plt.axis('equal')
plt.title('% of Total Drivers by City Type')
plt.savefig('drivers by city type.png')
```


![png](output_6_0.png)

