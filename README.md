# Heart-Healers
import React from "react"; import { motion } from "framer-motion"; import { Button } from "@/components/ui/button"; import { Card, CardContent } from "@/components/ui/card"; import { Heart, Users, Shield, MessageCircle } from "lucide-react";

export default function LandingPage() { return ( <div className="bg-gradient-to-b from-pink-50 to-white min-h-screen"> {/* Hero Section */} <section className="text-center py-20 px-4"> <motion.h1 initial={{ opacity: 0, y: -20 }} animate={{ opacity: 1, y: 0 }} transition={{ duration: 0.6 }} className="text-5xl font-bold text-pink-600 mb-4" > Heart Healers </motion.h1> <p className="text-lg text-gray-700 max-w-2xl mx-auto mb-6"> Where broken boys help broken girls and broken girls help broken boys heal together. Find support, share experiences, and move on with care. </p> <Button className="bg-pink-600 text-white px-6 py-3 rounded-2xl shadow-lg"> Start Free 3-Day Trial </Button> </section>

{/* How It Works */}
  <section className="py-16 px-6 max-w-6xl mx-auto">
    <h2 className="text-3xl font-semibold text-center text-pink-600 mb-12">
      How It Works
    </h2>
    <div className="grid md:grid-cols-3 gap-8">
      <Card className="shadow-xl">
        <CardContent className="p-6 text-center">
          <Users className="h-10 w-10 text-pink-600 mx-auto mb-4" />
          <h3 className="font-bold text-lg mb-2">Create Profile</h3>
          <p className="text-gray-600">Sign up and share your story. Stay anonymous until you’re ready to connect.</p>
        </CardContent>
      </Card>
      <Card className="shadow-xl">
        <CardContent className="p-6 text-center">
          <Heart className="h-10 w-10 text-pink-600 mx-auto mb-4" />
          <h3 className="font-bold text-lg mb-2">Smart Matching</h3>
          <p className="text-gray-600">We match you with someone based on your ex’s interests and compatibility.</p>
        </CardContent>
      </Card>
      <Card className="shadow-xl">
        <CardContent className="p-6 text-center">
          <MessageCircle className="h-10 w-10 text-pink-600 mx-auto mb-4" />
          <h3 className="font-bold text-lg mb-2">Heal Together</h3>
          <p className="text-gray-600">Chat, share, and help each other move forward with empathy and care.</p>
        </CardContent>
      </Card>
    </div>
  </section>

  {/* Features */}
  <section className="bg-pink-50 py-16 px-6">
    <h2 className="text-3xl font-semibold text-center text-pink-600 mb-12">
      Why Choose Heart Healers?
    </h2>
    <div className="grid md:grid-cols-3 gap-8 max-w-6xl mx-auto">
      <Card className="shadow-xl">
        <CardContent className="p-6 text-center">
          <Shield className="h-10 w-10 text-pink-600 mx-auto mb-4" />
          <h3 className="font-bold text-lg mb-2">Safe & Private</h3>
          <p className="text-gray-600">Your data and chats are secure with our strong privacy protection.</p>
        </CardContent>
      </Card>
      <Card className="shadow-xl">
        <CardContent className="p-6 text-center">
          <Heart className="h-10 w-10 text-pink-600 mx-auto mb-4" />
          <h3 className="font-bold text-lg mb-2">Empathy First</h3>
          <p className="text-gray-600">We focus on healing, not dating—building trust and comfort.</p>
        </CardContent>
      </Card>
      <Card className="shadow-xl">
        <CardContent className="p-6 text-center">
          <Users className="h-10 w-10 text-pink-600 mx-auto mb-4" />
          <h3 className="font-bold text-lg mb-2">Supportive Community</h3>
          <p className="text-gray-600">Join a network where everyone understands your pain and helps you heal.</p>
        </CardContent>
      </Card>
    </div>
  </section>

  {/* Pricing */}
  <section className="py-16 px-6 max-w-4xl mx-auto text-center">
    <h2 className="text-3xl font-semibold text-pink-600 mb-12">Pricing</h2>
    <Card className="shadow-xl">
      <CardContent className="p-8">
        <h3 className="text-2xl font-bold mb-4">Free Trial</h3>
        <p className="text-gray-600 mb-6">3 days of free access to explore Heart Healers.</p>
        <h3 className="text-2xl font-bold mb-4">₹199/month</h3>
        <p className="text-gray-600 mb-6">Continue your healing journey with unlimited support and matching.</p>
        <Button className="bg-pink-600 text-white px-6 py-3 rounded-2xl shadow-lg">
          Subscribe Now
        </Button>
      </CardContent>
    </Card>
  </section>

  {/* FAQ */}
  <section className="bg-pink-50 py-16 px-6">
    <h2 className="text-3xl font-semibold text-center text-pink-600 mb-12">FAQ</h2>
    <div className="max-w-3xl mx-auto space-y-6">
      <div>
        <h4 className="font-bold">Is this a dating app?</h4>
        <p className="text-gray-600">No, Heart Healers is focused on emotional healing, not dating.</p>
      </div>
      <div>
        <h4 className="font-bold">How does matching work?</h4>
        <p className="text-gray-600">We use shared experiences and ex’s interests to connect people who can relate.</p>
      </div>
      <div>
        <h4 className="font-bold">Is my data safe?</h4>
        <p className="text-gray-600">Absolutely. We prioritize safety, privacy, and confidentiality.</p>
      </div>
    </div>
  </section>

  {/* Call to Action */}
  <section className="py-20 text-center px-6">
    <h2 className="text-4xl font-bold text-pink-600 mb-6">
      Ready to Heal Your Heart?
    </h2>
    <Button className="bg-pink-600 text-white px-6 py-3 rounded-2xl shadow-lg">
      Join Heart Healers Today
    </Button>
  </section>

  {/* Footer */}
  <footer className="bg-pink-600 text-white py-6 text-center">
    <p>© {new Date().getFullYear()} Heart Healers. All rights reserved.</p>
  </footer>
</div>

); }


