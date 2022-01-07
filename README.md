# postech

#import the functions to resolve the signal stream
from pylsl import StreamInlet, resolve_stream

#resolve_stream 함수를 통해 스트림의 이름 명시
print("#looking for an available OpenSignals stream.. ")
os_stream = resolve_stream("name","OpenSignals")

#inlet을 생성해 stream으로부터 tlsghtoavmfdmf qkesmsek
inlet = StreamInlet(os_stream[0])

#
while Ture:
  sample,timestamp=inlet.pull_sample()
  print(timestamp,sample)
