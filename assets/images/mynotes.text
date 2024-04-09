import 'dart:ffi';

import 'package:flutter/material.dart';

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        backgroundColor: const Color.fromRGBO(12, 12, 12, 1),
        body: Stack(
          children: [
            const Positioned(
              top: 25,
              left: 20,
              child: Icon(
                Icons.arrow_back,
                color: Colors.white,
                size: 30,
              ),
            ),
            const Positioned(
              top: 25,
              right: 20,
              child: Icon(
                Icons.settings,
                color: Colors.white,
                size: 30,
              ),
            ),
            Center(
              child: Column(
                mainAxisAlignment: MainAxisAlignment.center,
                children: [
                  const CircleAvatar(
                    radius: 60,
                    backgroundImage: AssetImage('assets/images/eren.jpeg'),
                  ),
                  const SizedBox(height: 10),
                  const Text(
                    'Eren Jaeger',
                    style: TextStyle(
                      fontSize: 24,
                      fontWeight: FontWeight.w600,
                      color: Colors.white,
                    ),
                  ),
                  const SizedBox(height: 1),
                  const Text(
                    'erenjaeger@rumbling.com',
                    style: TextStyle(
                      color: Colors.white,
                      fontSize: 15,
                    ),
                  ),
                  Container(
                    height: 50,
                    width: 300,
                    margin: const EdgeInsets.only(
                        left: 20, top: 20, right: 20, bottom: 10),
                    decoration: const BoxDecoration(
                      color: Color.fromRGBO(72, 30, 20, 1),
                      borderRadius: BorderRadius.all(Radius.circular(20)),
                    ),
                    child: Padding(
                      padding: const EdgeInsets.only(right: 15),
                      child: Row(
                        mainAxisAlignment: MainAxisAlignment.spaceBetween,
                        children: [
                          Padding(
                            padding: const EdgeInsets.only(left: 10),
                            child: Row(
                              children: const [
                                Icon(
                                  Icons.download,
                                  size: 30,
                                  color: Colors.blue,
                                ),
                                Padding(
                                  padding: EdgeInsets.only(left: 7),
                                  child: Text(
                                    'Download Manga',
                                    style: TextStyle(
                                      color: Colors.white,
                                      fontSize: 20,
                                      letterSpacing: 0.5,
                                    ),
                                  ),
                                ),
                              ],
                            ),
                          ),
                          const Icon(
                            Icons.arrow_forward,
                            color: Colors.blue,
                            size: 30,
                          )
                        ],
                      ),
                    ),
                  ),
                  // End of first container
                  // Layout Section
                  LayoutWidget(
                    text: 'Contact Author',
                    icon: Icons.mail_lock,
                    arrowShown: true,
                  ),
                  const SizedBox(height: 10),

                  LayoutWidget(
                    text: 'Other Books',
                    icon: Icons.book,
                    arrowShown: true,
                  ),
                  const SizedBox(height: 10),
                  LayoutWidget(
                    text: 'Character Dept',
                    icon: Icons.person,
                    arrowShown: true,
                  ),
                  const SizedBox(height: 10),
                  LayoutWidget(
                    text: 'Support Us',
                    icon: Icons.monetization_on,
                    arrowShown: true,
                  ),
                  const SizedBox(height: 10),

                  LayoutWidget(
                    text: 'Referrals',
                    icon: Icons.share,
                    arrowShown: true,
                  ),
                  const SizedBox(height: 10),

                  LayoutWidget(
                    text: 'Log Out',
                    icon: Icons.logout,
                    arrowShown: false,
                  ),

                  // End of second containern
                ],
              ),
            ),
          ],
        ),
      ),
    );
  }
}

// Widget Extraction Section
class LayoutWidget extends StatelessWidget {
  LayoutWidget(
      {required this.text, required this.icon, required this.arrowShown});
  final String text;
  final IconData icon;
  final bool arrowShown;

  @override
  Widget build(BuildContext context) {
    return Container(
      height: 45,
      width: 300,
      decoration: const BoxDecoration(
        color: Color.fromRGBO(24, 111, 101, 1),
        borderRadius: BorderRadius.all(Radius.circular(20)),
      ),
      child: Row(
        mainAxisAlignment: MainAxisAlignment.spaceBetween,
        children: [
          Padding(
            padding: const EdgeInsets.only(left: 10),
            child: Row(
              children: [
                Icon(
                  icon,
                  size: 30,
                  color: Colors.white,
                ),
                Padding(
                  padding: const EdgeInsets.only(left: 8.0),
                  child: Text(
                    text,
                    style: const TextStyle(
                      fontSize: 20,
                      color: Colors.white,
                      fontWeight: FontWeight.w300,
                    ),
                  ),
                )
              ],
            ),
          ),
          arrowShown
              ? const Padding(
                  padding: EdgeInsets.only(right: 10),
                  child: Icon(
                    Icons.arrow_forward,
                    size: 30,
                    color: Colors.white,
                  ),
                )
              : Container(),
        ],
      ),
    );
  }
}
