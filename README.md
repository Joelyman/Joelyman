import matplotlib.pyplot as plt

# Data
tahun = [2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023]
PDRB = [243456, 256789, 270123, 283456, 296789, 301234, 314567, 331890, 351857]
persentase_miskin = [12.34, 11.89, 11.45, 11.01, 10.57, 10.13, 9.69, 9.25, 7.72]
gini_ratio = [0.371, 0.369, 0.367, 0.365, 0.363, 0.361, 0.359, 0.357, 0.354]
IPM = [74.89, 75.34, 75.79, 76.24, 76.69, 77.14, 77.59, 78.04, 77.17]

# Plot
plt.figure(figsize=(10, 6))
plt.plot(tahun, PDRB, marker='o', label='PDRB (Miliar Rupiah)')
plt.plot(tahun, persentase_miskin, marker='o', label='Persentase Penduduk Miskin')
plt.plot(tahun, gini_ratio, marker='o', label='Gini Ratio')
plt.plot(tahun, IPM, marker='o', label='IPM')
plt.title('Tren Data Ekonomi dan Sosial 2015-2023')
plt.xlabel('Tahun')
plt.ylabel('Nilai')
plt.legend()
plt.grid(True)
plt.xticks(tahun)
plt.tight_layout()
plt.show()
