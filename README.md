# Text-classification-using-CNN-models
Đây là tất cả các file source code mô hình và dữ liệu dataset mà bọn em đã sử dụng để đưa vào bài tập lớn của nhóm bọn em. Dữ liệu đã được làm sạch và lưu lử file folder Twitter_1 và Twitter_2. Các file code sẽ có tên model đã code trên đấy và id của model để có thể theo dõi
Người dùng có thể tải file về thay đổi code ở đoạn load data để sử dụng các dataset đã làm sạch khác để huấn luyện cho mô hình phù hợp với ý muốn
File Preprocessing data dùng để làm sạch dữ liệu huấn luyện người dùng có thể tham khảo dể có thể làm sạch file dữ liệu huấn luyện của mình \n
Đối với data set 1 Twitter Sentiment cop đoạn code sau vào đoạn lấy file trong các file code mô hình \n
X_tr=pd.read_csv('Twitter_2/X_train_cleaned.csv',header=None,encoding='latin1')
Y_tr=pd.read_csv('Twitter_2/Y_train_cleaned.csv',header=None)
X_t=pd.read_csv('Twitter_2/X_test_cleaned.csv',header=None,encoding='latin1')
Y_t=pd.read_csv('Twitter_2/Y_test_cleaned.csv',header=None)
X_train = X_tr[0].astype(str).tolist()
X_test = X_t[0].astype(str).tolist()
Đối với dataset 2 Corona NLP cop đoạn code sau vào đoạn lấy file data trong các file code mô hình \n
df=pd.read_csv('Twitter_3/data_train.csv',header=None)
df = df.iloc[1:]
df_test=pd.read_csv('Twitter_3/data_test.csv',header=None)
df_test = df_test.iloc[1:]
X_train=df.iloc[:,0]
Y_tr=df.iloc[:,2]
X_test=df_test.iloc[:,0]
Y_t=df_test.iloc[:,2]
