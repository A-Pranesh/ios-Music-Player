# ios-Music-Player
import React from 'react';
import { StyleSheet, View, Text } from 'react-native';
 
 export default class AudioPlayer extends React.Component{
 	render() {
 		const name = '01 - Singapenne - Bigil';

 		return (
 				<View style = {styles.outerContainer}>
 					<View style = {styles.innerContainer} />
 					<Text style = {styles.title}>
 						<Text style = {styles.subtitle}>Playing:</Text> {name}
 					</Text>
 				</View>
 			);
 	}
 }


const styles = StyleSheet.create({
	outerContainer: {
		margin: 10,
		marginTop: 100,
		backgroundColor: '#e67e22',
		borderRadius: 5,
	},
	innerContainer: {
		backgroundColor: '#d35400',
		height: 50,
		width: 150,
		borderTopLeftRadius: 5,
    	borderBottomLeftRadius: 5,
	},
	title: {
		fontSize: 15,
		color: 'white',
		position: 'absolute',
		marginTop: 15,
		marginLeft: 10,
	},
	subtitle: {
		fontWeight: 'bold',
	},
});
