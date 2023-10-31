# baiktraltdidong
import { StatusBar } from 'expo-status-bar';
import { StyleSheet, Text, View, Image, TouchableOpacity } from 'react-native';

export default function App() {
  return (
    <View style={styles.container}>
      <View style={styles.head}>
        <View style={styles.backshare}>
          <Image source={require("../pj/assets/iconBack.png")}></Image>
          <Image source={require("../pj/assets/iconsh.png")}></Image>
        </View>
        <Image source={require("../pj/assets/img1.png")} style={[styles.img, { width: '100%', height: 420 }]} ></Image>

      </View>
      <View style={styles.foot}>
        <View style={styles.title}>
          <View style={{ flexDirection: 'column' }}>
            <Text style={styles.label}>Go for a walk</Text>
            <Text style={styles.label}>and feed the dog</Text>
          </View>
          <Image style={styles.heart} source={require("../pj/assets/like.png")}></Image>
        </View>
        <View>
          <Text style={styles.content}>Leaving for a week, French Bulldog Wilfred needs help feeding twice a day
          and walk from 26 to 30 September.
          I bought food, it will be easy.</Text>
        </View>
        <View>
          <View style={styles.info}>
            <Image source={require("../pj/assets/iconWallet.png")}></Image>
            <Text style={styles.text}>Reward 34$</Text>
          </View>
          <View style={styles.info}>
            <Image source={require("../pj/assets/iconGeo.png")}></Image>
            <Text style={styles.text}>3 HERALD</Text>
            <Text style={{fontSize:14, color:'#31313180', paddingLeft:10, fontWeight:'400'}}>400m from you</Text>
          </View>
        </View>
        <View style={styles.bottom}>
          <TouchableOpacity style={styles.chat}>
            <Image style={styles.chatbox} source={require("../pj/assets/Chat.png")}></Image>
          </TouchableOpacity>
          <TouchableOpacity style={styles.rep}>
            <Text style={styles.ans}>Respond</Text>
          </TouchableOpacity>
        </View>
      </View>
    </View>
  );
} const styles = StyleSheet.create({
  container: {
    flex: 1,
  },
  backshare: {
    flexDirection: 'row',
    justifyContent: 'space-between',
    position: 'absolute',
    top: 14,
    zIndex: 1,
  },
  head: {
    flex: 1,
    paddingBottom: 28,
  },
  foot: {
    flex: 1,
    paddingHorizontal: 25,
    paddingTop: 30,
  },
  title: {
    flexDirection: 'row',
    justifyContent: 'space-between',
  },
  label: {
    fontSize: 26,
    fontWeight: '800',
  },
  heart: {
    marginTop: 10,
  },
  content:{
    marginTop:10,
    fontSize: 17,
    fontWeight: '400',
    textAlign:'justify',
  },
  info:{
    marginTop:15,
    flexDirection:'row',
  },
  text:{
    fontSize:15,
    paddingLeft:10,
    fontWeight:'600',
  },
  bottom:{
    height:60,
    marginTop:50,
    flexDirection:'row',
  },
  rep:{
    width:251,
    backgroundColor:'#A58EFF',
    paddingVertical:20,
    borderRadius:12,
  },
  ans:{textAlign:'center',
    color:'#fff',
    fontSize:15,
    lineHeight:18,
    fontWeight:'500',
  },
});
