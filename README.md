# fft.png
[h, fs] = audioread ('melody.wav') h = fft (h); cốt truyện (abs (h)) nhân vật N = fs% số điểm FFT transform = fft (h, N) / N; magTransform = abs (biến đổi);  faxis = linspace (-fs / 2, fs / 2, N); cốt truyện (faxis, fftshift (magTransform)); xlabel ('Tần số (Hz)')  % nội dung tần suất xem lên đến một nửa tỷ lệ lấy mẫu: trục ([0 chiều dài (fax) / 2, 0 max (magTransform)])   % thay đổi nhãn đánh dấu của biểu đồ từ ký hiệu khoa học thành dấu phẩy động:  xt = get (gca, 'XTick');   set (gca, 'XTickLabel', sprintf ('%. 0f |', xt))
