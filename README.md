# PyCity Schools Analysis 

This is an analysis of fictitious district-wide standardized test results. Data is contains student's math and reading scores, as well as various information on the schools they attend. The purpose is to uncover trends in school performance using the pandas library for Python.

## Key Insights: 
* Top performing schools are all smaller charter schools with smaller per student budgets. 
* Bottom performing schools are larger district schools that have larger per student budgets. 
* There seems to be a performance and spending threshold at school size about 2,000 students.  

## Tools:
pandas<br>
Jupyter Notebook
<br>
<br>
# Analysis
Key insights are supported by the findings below. For full view of code and results see [PyCitySchools.ipynb](PyCitySchools.ipynb).
<br>
<br>  
## District Summary
This is a high level snapshot of the district's key metrics.
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
      <th>Total Schools</th>
      <th>Total Students</th>
      <th>Total Budget</th>
      <th>Average Math Score</th>
      <th>Average Reading Score</th>
      <th>% Passing Math</th>
      <th>% Passing Reading</th>
      <th>% Overall Passing</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>15</td>
      <td>39,170</td>
      <td>$24,649,428</td>
      <td>79</td>
      <td>82</td>
      <td>0.92</td>
      <td>1.00</td>
      <td>0.92</td>
    </tr>
  </tbody>
</table>
</div>
<br>
<br>

## Top Performing Schools
Table shows top 5 performing schools based on % Overall Passing.



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
      <th></th>
      <th>Total Students</th>
      <th>Total School Budget</th>
      <th>Average Reading Score</th>
      <th>Average Math Score</th>
      <th>Per Student Budget</th>
      <th>% Passing Math</th>
      <th>% Passing Reading</th>
      <th>% Overall Passing</th>
    </tr>
    <tr>
      <th>School Name</th>
      <th>School Type</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Cabrera High School</th>
      <th>Charter</th>
      <td>1858</td>
      <td>$1,081,356.0</td>
      <td>84</td>
      <td>83</td>
      <td>$582.0</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>1.00</td>
    </tr>
    <tr>
      <th>Griffin High School</th>
      <th>Charter</th>
      <td>1468</td>
      <td>$917,500.0</td>
      <td>84</td>
      <td>83</td>
      <td>$625.0</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>1.00</td>
    </tr>
    <tr>
      <th>Holden High School</th>
      <th>Charter</th>
      <td>427</td>
      <td>$248,087.0</td>
      <td>84</td>
      <td>84</td>
      <td>$581.0</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>1.00</td>
    </tr>
    <tr>
      <th>Pena High School</th>
      <th>Charter</th>
      <td>962</td>
      <td>$585,858.0</td>
      <td>84</td>
      <td>84</td>
      <td>$609.0</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>1.00</td>
    </tr>
    <tr>
      <th>Shelton High School</th>
      <th>Charter</th>
      <td>1761</td>
      <td>$1,056,600.0</td>
      <td>84</td>
      <td>83</td>
      <td>$600.0</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>1.00</td>
    </tr>
  </tbody>
</table>
</div>
<br>
<br>

## Bottom Performing Schools
Table shows bottom 5 performing schools based on % Overall Passing.

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
      <th></th>
      <th>Total Students</th>
      <th>Total School Budget</th>
      <th>Average Reading Score</th>
      <th>Average Math Score</th>
      <th>Per Student Budget</th>
      <th>% Passing Math</th>
      <th>% Passing Reading</th>
      <th>% Overall Passing</th>
    </tr>
    <tr>
      <th>School Name</th>
      <th>School Type</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Figueroa High School</th>
      <th>District</th>
      <td>2949</td>
      <td>$1,884,411.0</td>
      <td>81</td>
      <td>77</td>
      <td>$639.0</td>
      <td>0.88</td>
      <td>1.00</td>
      <td>0.88</td>
    </tr>
    <tr>
      <th>Ford High School</th>
      <th>District</th>
      <td>2739</td>
      <td>$1,763,916.0</td>
      <td>81</td>
      <td>77</td>
      <td>$644.0</td>
      <td>0.89</td>
      <td>1.00</td>
      <td>0.89</td>
    </tr>
    <tr>
      <th>Hernandez High School</th>
      <th>District</th>
      <td>4635</td>
      <td>$3,022,020.0</td>
      <td>81</td>
      <td>77</td>
      <td>$652.0</td>
      <td>0.89</td>
      <td>1.00</td>
      <td>0.89</td>
    </tr>
    <tr>
      <th>Huang High School</th>
      <th>District</th>
      <td>2917</td>
      <td>$1,910,635.0</td>
      <td>81</td>
      <td>77</td>
      <td>$655.0</td>
      <td>0.89</td>
      <td>1.00</td>
      <td>0.89</td>
    </tr>
    <tr>
      <th>Johnson High School</th>
      <th>District</th>
      <td>4761</td>
      <td>$3,094,650.0</td>
      <td>81</td>
      <td>77</td>
      <td>$650.0</td>
      <td>0.89</td>
      <td>1.00</td>
      <td>0.89</td>
    </tr>
  </tbody>
</table>
</div>
<br>
<br>

## Scores by School Size
Table breaks down school performance based on relative school size within the district. 

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
      <th>Average Math Score</th>
      <th>Average Reading Score</th>
      <th>% Passing Math</th>
      <th>% Passing Reading</th>
      <th>% Overall Passing</th>
    </tr>
    <tr>
      <th>School Size</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Small</th>
      <td>83</td>
      <td>84</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>1.00</td>
    </tr>
    <tr>
      <th>Medium</th>
      <td>78</td>
      <td>82</td>
      <td>0.91</td>
      <td>1.00</td>
      <td>0.91</td>
    </tr>
    <tr>
      <th>Large</th>
      <td>77</td>
      <td>81</td>
      <td>0.89</td>
      <td>1.00</td>
      <td>0.89</td>
    </tr>
  </tbody>
</table>
</div>
<br>
<br>

## Conclusion 
It would be worth digging into the different curriculum and procedures between the types of schools. It would also be worth looking at any differences in the students' needs in the different types of schools. This may account for the per student budget differences. Furthermore, there needs to be a cost/benefit analysis done on splitting up larger schools. It seems the district could reduce spending and increase student outcomes by instilling a goal of no more than 2,000 students in a school.  
<br>

# Contact Information: 
### Hope Neely
Email: [hope.neely@gmail.com](hope.neely@gmail.com)<br>
LinkedIn : [https://www.linkedin.com/in/hopeneely/](https://www.linkedin.com/in/hopeneely/)