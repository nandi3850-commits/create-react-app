import { Card, CardContent } from "@/components/ui/card";
import { motion } from "framer-motion";

export default function RecognitionPyramid() {
  return (
    <div className="flex flex-col items-center p-6 bg-gray-50 min-h-screen">
      <h1 className="text-3xl font-bold mb-6 text-gray-800">Recognition & Rewards Pyramid</h1>
      <div className="relative w-full max-w-2xl">
        {/* Pyramid Shape */}
        <div className="flex flex-col items-center space-y-4">
          {/* Annual Awards */}
          <motion.div
            whileHover={{ scale: 1.05 }}
            className="w-1/2 bg-yellow-500 text-white text-center p-4 rounded-2xl shadow-lg"
          >
            <h2 className="text-xl font-semibold">Annual Awards</h2>
            <p className="text-sm">Elite Excellence & Long-term Achievement</p>
          </motion.div>

          {/* Excellerator Awards */}
          <motion.div
            whileHover={{ scale: 1.05 }}
            className="w-2/3 bg-purple-500 text-white text-center p-4 rounded-2xl shadow-lg"
          >
            <h2 className="text-xl font-semibold">Excellerator Awards</h2>
            <p className="text-sm">Strategic Impact & Innovation</p>
          </motion.div>

          {/* Spot Awards */}
          <motion.div
            whileHover={{ scale: 1.05 }}
            className="w-4/5 bg-blue-500 text-white text-center p-4 rounded-2xl shadow-lg"
          >
            <h2 className="text-xl font-semibold">Spot Awards</h2>
            <p className="text-sm">Instant Recognition for High Performance</p>
          </motion.div>

          {/* Milestone Awards */}
          <motion.div
            whileHover={{ scale: 1.05 }}
            className="w-10/12 bg-green-500 text-white text-center p-4 rounded-2xl shadow-lg"
          >
            <h2 className="text-xl font-semibold">Milestone Awards</h2>
            <p className="text-sm">Celebrating Loyalty & Tenure</p>
          </motion.div>

          {/* Everyday Recognition */}
          <motion.div
            whileHover={{ scale: 1.05 }}
            className="w-full bg-gray-700 text-white text-center p-4 rounded-2xl shadow-lg"
          >
            <h2 className="text-xl font-semibold">Everyday Recognition</h2>
            <p className="text-sm">Daily Appreciation & Connection</p>
          </motion.div>
        </div>
      </div>
      <div className="mt-8 max-w-2xl">
        <Card className="shadow-md">
          <CardContent className="p-4 text-gray-700">
            <p className="mb-2"><strong>Why this works:</strong></p>
            <ul className="list-disc ml-5 space-y-1 text-sm">
              <li>Grounded in academic research (Maslow, Herzberg, Deci & Ryan).</li>
              <li>Validated by Deloitte, PwC, and O.C. Tanner practices.</li>
              <li>Inclusive design: from everyday connection to elite excellence.</li>
              <li>Boosts engagement, retention, and organizational culture.</li>
            </ul>
          </CardContent>
        </Card>
      </div>
    </div>
  );
}
