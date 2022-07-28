import codecademylib3_seaborn
from matplotlib import pyplot as plt
import pandas as pd
import seaborn as sns

df = pd.read_csv('WorldCupMatches.csv')

df['Total Goals'] = df['Home Team Goals'] + df['Away Team Goals']

# Setting styles
sns.set_style('whitegrid')

sns.set_context('poster', font_scale = 0.5)

f, ax = plt.subplots(figsize = (12,7))

ax = sns.barplot(data = df, x = 'Year', y = 'Total Goals')

ax.set_title('Total Goals by Year')

plt.show()

# Box plot

df_goals = pd.read_csv('goals.csv')
print(df_goals.head())

sns.set_context('notebook', font_scale = 0.75)

f, ax2 = plt.subplots(figsize = (12,7))

ax2 = sns.boxplot(data = df_goals, x = 'year', y = 'goals', palette = 'Spectral')

plt.title('Goals per Year')
plt.show()
